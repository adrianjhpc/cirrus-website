---
layout: section
title: Cirrus Service Status
summary: Up to date status of the Cirrus service
---

## Known Issues

### Current Issues

#### Tuesday 22nd October

As part of the emergency maintenance last week we resolved an issue with the incorrect version of the HPE MPT library being loaded on the compute nodes by default.

The correct version of HPE MPT (2.18) is now being loaded by default on the compute nodes but this has consequences for the use of the `mpiexec_mpt` command in your job submission scripts if you are using the default version of HPE MPT:

1. You must use the `-ppn` option when using the `mpiexec_mpt` command otherwise you will see an error similar to: *mpiexec_mpt error: Need 36 processes but have only 1 left in PBS_NODEFILE*

2. When using the `mpiexec_mpt` command, the `-ppn` option must come before the `-n` option otherwise you will see an error similar to: *MPT ERROR: Not enough slots from job scheduler for requested ranks*

You will need to pay attention to these points if your job submission script contains:

```
module load mpt
```

or 

```
module load mpt/2.18
```

or loads a package that loads the default version of HPE MPT.

If you are using Intel MPI, then your job submission scripts should be unaffected.

### Recent Issues

No recent issues

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

No maintenance planned





