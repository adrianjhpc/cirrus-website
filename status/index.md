---
layout: section
title: Cirrus Service Status
summary: Up to date status of the Cirrus service
---

## Known Issues

### Current Issues

**2018-11-23** We are investigating an issue with Lustre mounts on the compute nodes that may cause some applications that use MPI-IO to fail with error messages similar to:

```
This requires fcntl(2) to be implemented. As of 8/25/2011 it is not. Generic MPICH Message: File locking failed in ADIOI_Set_lock(fd C,cmd F_SETLKW/7,type F_RDLCK/0,whence 0) with return value FFFFFFFF and errno 26. 
- If the file system is NFS, you need to use NFS version 3, ensure that the lockd daemon is running on all the machines, and mount the directory with the 'noac' option (no attribute caching). 
- If the file system is LUSTRE, ensure that the directory is mounted with the 'flock' option. 
ADIOI_Set_lock:: Function not implemented 
ADIOI_Set_lock:offset 0, length 32 
application called MPI_Abort(MPI_COMM_WORLD, 1) - process 0 
```

### Recent Issues

- **2018-11-21** Issues with PBS configuration was stopping jobs from starting. Issue resolved just after 11pm 2018-11-21.

## Service Calendar and Maintenance

We maintain a calendar for the Cirrus service that lists upcoming events (such
as training courses and maintenance sessions):

- [Cirrus Service Calendar](calendar.html)

We keep maintenance downtime to a minimum on the service but do occaisionally
need to perform essential work on the system. Maintenance sessions are used to 
ensure that:

* software versions are kept up to date;
* firmware levels on HPE and third-party peripheral equipment are kept up to date;
essential security patches are applied;
* failed/suspect hardware can be replaced;
* new software can be installed;
periodic essential maintenance on HPE electrical and mechanical support equipment (refrigeration systems, air blowers and power distribution units) can be undertaken safely.

Additional maintenance sessions can be scheduled for major hardware or software updates; major upgrades to facility plant and infrastructure; acceptance testing following major service upgrades and statutory electrical testing.

### Upcoming Maintenance Sessions

#### 0900-1700 GMT, 21 November 2018 

Login, Data Services Node (DSN) and Compute Nodes will all be unavailable during this maintenance session. 

Activities planned: 

- Change ncpus available per node from 72 to 36
- Remove default node exclusive for standard compute nodes 
- Reconfiguration of hardware distribution in Cirrus racks
- Enable additional system monitoring

Impact of changes on users: 

- Job scripts that request ncpus > 36 will no longer work on Cirrus. These scripts should be modified 
  to set ncpus=36
- Jobs that want node exclusive access *must* specify `-l place=scatter:excl` as an option to `qsub` 
  (either on the command line or as `#PBS -l place=scatter:excl` in their job submission script


