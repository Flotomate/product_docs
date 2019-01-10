*****************************
Disaster Recovery Setup Guide
*****************************

Disaster recovery is an automated process to replicate the database of
the main server in a remote server.

**Requirements**:

-  A pre-configured server as the remote server with a user having sudo
   rights.

-  Static IPs for both main and remote servers.

**Steps to Initiate Disaster Recovery**

**Note:** For demonstration sake, you would consider IP addresses of
main and remote as: *Main-server: 192.168.1.111* and *Remote-server:
192.168.1.109*.

1. Create authentication SSH-Keygen keys on the main server
   (*192.168.1.111*).

   a. Run the following commands.

      .. _reco-1:

      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/recovery/RECO-1.png
          :align: center
          :alt: figure 1


      .. code-block:: ssh-keygen -t rsa

This generates a pair of public keys.

2. Create .ssh directory in the remote server (192.168.1.109).

   a. Use ssh from main server to connect to the remote server using
      [remote server username] and create .ssh directory using the
      following command.

      .. _reco-2:

      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/recovery/RECO-2.png
          :align: center
          :alt: figure 2

      .. code-block:: ssh [remote server username]@192.168.1.109 mkdir -p .ssh

   b. You will be asked for the password of the remote server’s user
      account; please type in the password.

3. Upload generated public keys to remote server (192.168.1.109).

   a. We will upload the new generated public key in the main server on
      the remote server using the following command.

      .. _reco-3:

      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/recovery/RECO-3.png
          :align: center
          :alt: figure 3

      .. code-block:: cat .ssh/id_rsa.pub \| ssh [remote server username]@192.168.1.109
                      'cat >> .ssh/authorized_keys'

   b. You will be asked for the password of the remote server’s user
      account; provide the password.

4. Set permissions in remote server (192.168.1.109) and a directory
   where the recovery will happen.

   a. Log in to the remote server and run the following commands.

      .. code-block:: sudo cp -R ~/.ssh /root/
                      sudo -i
                      chmod 700 ~/.ssh
                      chmod 640 ~/.ssh/authorized_keys
                      mkdir /opt/dr

5. Login from main (192.168.1.111) to remote (192.168.1.109) without
   using password.

   .. code-block:: ssh [remote server username]@192.168.1.109

You can now login to the remote server without a password.

6. Now we will create a cron job in the main server (192.168.1.111) as
   the root user.

   .. code-block:: crontab -l > mycron
                   echo "0 \* \* \* \* sh /opt/utility/dr.sh {remote machine ip}" >>
                   mycron
                   crontab mycron
                   rm mycron