**********************
Batch Patch Deployment
**********************

When deploying Patches over a large number of computers, it may cause unwanted consumption of network bandwidth. We have created Batch Deployment
to overcome this problem. 

Batch Deployment allows you to deploy Patches in a specific number of PCs at a time. Batch Deployment is by default turned off. 

**To Configure Batch Deployment:**

- Go to **Admin** (A Navigation Tab) >> **Batch Deploy Configuration** (Patch/Package Deployment).

- The Batch Deploy Configuration page opens. Here you get the following options:

    .. _P-batch-1:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-BATCH-1.png
        :align: center
        :alt: figure 1
  
  a. During a Patch Deployment cycle, the deployment process is broken down into smaller units. For example; deployment in 100 computers
     can be divided into 25 computers at a time; at a time, only 25 computers will receive the deployment command. The **Batch Size**
     decides the size of each unit.

  b. Batch Interval is the time between two Batches (units). For example; you can deploy Batches every 2 hours. 

  c. You can decide how 
   