---
layout: page
---

Hardware
========

The Cirrus facility is based around a SGI ICE XA 280 node cluster.

Intel ICE XA Cluster
--------------------

The Cirrus compute provision consists of 280 compute nodes connected
together by a single Infiniband fabric.

There are 3 login nodes that share a common software environment and
file system with the compute nodes.

### Compute Nodes

Cirrus compute nodes each contain two 2.1 GHz, 18-core Intel Xeon
E5-2695 (Broadwell) series processors. Each of the cores in these
processors support 2 hardware threads (Hyperthreads), which are enabled
by default.

The compute nodes on Cirrus have 256 GB of memory shared between the two
processors. The memory is arranged in a non-uniform access (NUMA) form:
each 18-core processor is a single NUMA region with local memory of 128
GB. Access to the local memory by cores within a NUMA region has a lower
latency than accessing memory on the other NUMA region.

There are three levels of cache, configured as follows:

-   L1 Cache 32 KB Instr., 32 KB Data (per core)
-   L2 Cache 256 KB (per core)
-   L3 Cache 45 MB (shared)

There are 280 compute nodes on Cirrus giving a total of 10,080 cores.
When employing hyperthreads, the core count doubles to 20,160.

Infiniband fabric
-----------------

The system has a single infiniband (IB) fabric and every compute node
and login node has a single ib0 interface. The IB interface is FDR, with
a bandwidth of 54.5 Gb/s. The Lustre servers have two connections to the
IB fabric and all Lustre file system IO traverses the IB fabric.

Filesystems and Data Infrastructure
-----------------------------------

There is currently a single file system available on Cirrus: /lustre is
a Lustre parallel file system desgined to give high read/write bandwidth
for parallel calculations running on Cirrus.

The Lustre file system has  a total of 406 TiB available.
The cluster login and compute nodes mount the storage as /lustre, and
all home directories are available on all nodes.

The compute nodes are diskless. Each node boots from a cluster
management noded called the Rack Leader and NFS mounts the root file
system from this management node.

*Note:* There are currently no backups of data on Cirrus as backing up
the whole Lustre file system would adversely affect the performance of
write access for simulations. The nature of the Lustre parallel file
system means that there is data resiliance in the case of failures of
individual hardware components. However, we strongly advise that you
keep copies of any critical data on different systems.

Parallel I/O
------------

For a description of the terms associated with Lustre file systems
please see the description on Wikipedia:

-   [Lustre File Systems
    Description](https://en.wikipedia.org/wiki/Lustre_(file_system))

The default striping on the Lustre filesystem is 1 stripe, and the
default stripe size is 1 MiB.

