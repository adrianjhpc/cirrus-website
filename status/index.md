---
layout: section
title: Cirrus Service Status
summary: Up to date status of the Cirrus service
---

## Known Issues

### Current Issues

- No open issues

### Recent Issues

- No recent issues

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

### Upcoming Maintenance Sessions

#### 0900-1700 BST, 22 August 2018

Login, Data Services Node (DSN) and Compute Nodes will all be unavailable during this maintenance session.

**Activites planned:**
* Updates to PBS queue layouts to improve capacity control
* Installation of squashfs-tools to support pulling Singularity container images from DockerHub
* Installation of Intel 18 compilers and libraries
* Removal of Spack modulefiles path from default MODULEPATH to improve clarity of which software modules are available

**Impact of changes on users:**

The largest impact on users will come from the change of the default MODULEPATH. This change will result in
a large number of current software modules no longer being visible by default to users. This should improve the
clarity in use of software modules for users as:

* Only the key software modules will be visible to users by default
* Large numbers of duplicate software modules will no longer be visible by default

If users wish to return to the current view of software modules, they can use the `module load spack` command to
make all possible software modules visible.

Installation of squashfs-tools will allow users to pull container images from DockerHub on the Cirrus login
nodes and automatically convert them to Singularity container images. This gives users access to a large library
of existing container images for use on Cirrus.

The Intel 18 compilers and libraries will provide users with access to the lastest version of the Intel compilers
and libraries on Cirrus.
