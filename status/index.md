---
layout: section
title: Cirrus Service Status
summary: Up to date status of the Cirrus service
---

## Known Issues
No known issues

### Current Issues
No current issues

### Scheduled Maintenance
**At-Risk Maintenance Session Wednesday 5th August 0900-1300**

Our system team will be updating the Slurm scheduler configuration this during this maintenance window. There is a slight risk that during scheduler reconfiguration user job submission will stall briefly or fail. If you experience issues, please retry after a few minutes.

During the maintenance, the job size limits and available QoS will change, and we will update the documentation accordingly. 

If you have any questions please let us know. 


### Recent Issues

### Thursday 25th June 14:30

We are pleased to announce that Cirrus is now available to all users.

There is important information contained within this message so please read it completely before connecting to Cirrus.
* New access arrangement: SSH Passphrase and Password
* New Operating System: RHEL 8.1
* New Batch Scheduler: Slurm

**Access to Cirrus:**

Cirrus users are now required to use two credentials to access the service: an SSH key with a passphrase and their Cirrus password. It is imperative that users do not reuse a previously used password or SSH key with passphrase. All users will be asked to verify their SAFE accounts and we request that academic users use their UK home institutional email address for their SAFE account. If you are an academic user and do not have a UK academic email address (.ac.uk), then we will require confirmation from you PI that you are an active collaborator within the project before we can enable your access. Industrial users will be added to the access list.

New documentation describing this process is available at: [https://www.cirrus.ac.uk/docs/logging_on](https://www.cirrus.ac.uk/docs/logging_on)

**New Operating System**

The Operating System on Cirrus has been upgraded and is now RHEL 8.1 on the Cirrus login nodes.
This means that you may need to recompile your codes.
Updated documentation can be found at:  [https://cirrus.readthedocs.io/en/master/user-guide/development.html](https://cirrus.readthedocs.io/en/master/user-guide/development.html)


**New Batch Scheduling System**

Slurm has replaced PBS Pro as the Batch Scheduler on Cirrus.
This means that you will have to create new submission scripts before submitting jobs to the compute nodes.
Documentation including basic Slurm commands, resource limits and example job submission scripts can be found at:
[https://cirrus.readthedocs.io/en/master/user-guide/batch.html](https://cirrus.readthedocs.io/en/master/user-guide/batch.html)

We are anticipating a large number of Service Desk requests and we ask for your patience over the next few days but we will endeavour to resolve your requests as quickly as possible.

Please contact the Cirrus Service Desk if you have any concerns regarding this or require assistance accessing Cirrus and apologies for the inconvenience caused by this extended outage.


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

There is an 'At-Risk' Session provisionally booked every Wednesday from 1000 - 1200. 
A user mailing will be sent if any work is going to take place which may impact users.





