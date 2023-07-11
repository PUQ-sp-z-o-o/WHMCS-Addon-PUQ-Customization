# IP Pools

To enable the provision of virtual machines with virtual IP addresses, both IPv4 and IPv6, the configuration of an IP Pool is available.

An IP Pool is an abstract object that contains the following information:

- Server: The Proxmox server within the WHMCS system for which this pool will be active.
- Type: The type of the pool, which can be IPv4 or IPv6.
- Bridge and VLAN: Corresponding parameters that will be configured on the virtual machine if it receives an IP from this pool. (Please note that the addressing must be available on this Bridge and VLAN.)
- Gateway: The default gateway that will be configured on the virtual machine.
- Mask: The subnet mask that will be configured on the virtual machine.
- DNS1/DNS2: The DNS servers that will be configured on the virtual machine.
- Addresses: The range of addresses included in this pool. Please note that the Gateway will be excluded from the pool but will be listed as an occupied IP if it is part of the pool.

By configuring an IP Pool, you can streamline the allocation of virtual IP addresses for your virtual machines, ensuring efficient network management and connectivity within the Proxmox environment.

[![image-1689073685559.png](https://doc.puq.info/uploads/images/gallery/2023-07/scaled-1680-/image-1689073685559.png)](https://doc.puq.info/uploads/images/gallery/2023-07/image-1689073685559.png)

When viewing the list of IP pools, you will find information about the pool's size and its utilization. Additionally, there is a button available to view the services associated with IP addresses from that pool.

The size of the pool indicates the total number of available IP addresses within it, while the utilization provides insights into how many IP addresses have been allocated or are in use.

To gain further visibility into the services utilizing IP addresses from a particular pool, you can click on the designated button. This will provide you with a comprehensive overview of the services and associated virtual machines that currently utilize IP addresses from that specific pool. By accessing this information, you can effectively manage and monitor IP address allocation within your infrastructure.

[![image-1689073711513.png](https://doc.puq.info/uploads/images/gallery/2023-07/scaled-1680-/image-1689073711513.png)](https://doc.puq.info/uploads/images/gallery/2023-07/image-1689073711513.png)

[![image-1689073699626.png](https://doc.puq.info/uploads/images/gallery/2023-07/scaled-1680-/image-1689073699626.png)](https://doc.puq.info/uploads/images/gallery/2023-07/image-1689073699626.png)