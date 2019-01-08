---
layout: section
title: Cirrus Service Status
summary: Up to date status of the Cirrus service
---

## Known Issues

### Current Issues

- Our systems team have encountered issues with the InfiniBand network not coming back online following the maintenance on Monday 7th January. This affects all clusters Cirrus, GSEG and EGDP.

- We are investigating the issue and are in communication with HPE in order to resolve the issue as soon as possible.
Work overnight conducted by HPE to correct the InfiniBand issue have been unsuccessful. As a result HPE have now escalated this issue to their backline engineering team.

- There is currently no estimated resolution time and we are continuing to work with HPE to correct the issue, and will provide updates here as they become available to us.

- Meantime the system is unavailable to all users.  We apologise for the inconvenience this may cause.


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

### Upcoming Maintenance Sessions

#### 0900-1700 GMT, 7 January 2019

Electrical work is taking place at the ACF datacentre. All Cirrus nodes (login, data services, compute) will be unavailable during this time.


#### Changes made during Recent Maintenance Sessions

##### 0900-1700 GMT, 21 November 2018 

- Change ncpus available per node from 72 to 36
- Remove default node exclusive for standard compute nodes 
- Reconfiguration of hardware distribution in Cirrus racks
- Enable additional system monitoring

Impact of changes on users: 

- Job scripts that request ncpus > 36 will no longer work on Cirrus. These scripts should be modified 
  to set ncpus=36
- Jobs that want node exclusive access *must* specify `-l place=scatter:excl` as an option to `qsub` 
  (either on the command line or as `#PBS -l place=scatter:excl` in their job submission script


