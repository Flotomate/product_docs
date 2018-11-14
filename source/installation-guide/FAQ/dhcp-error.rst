.. _question2:

*********************************************************************************************************
Why CMDB update of existing Assets using Polling (Agent-less discovery) doesn't work using DHCP protocol?
*********************************************************************************************************

In a network using the DHCP protocol, IPs are dynamically allocated by a server. The IPs of machines change automatically
which are not captured by the system during agent-less discovery; this results in failure when existing assets are discovered again using polling.
To overcome this problem, you have to configure DNS in the product.

Learn :ref:`how to configure DNS <DNS Configuration>`.
