---
layout: section
title: Cirrus Service Status
summary: Up to date status of the Cirrus service
---

## Known Issues

### Current Issues




#### Cirrus Service Available: Thursday 25th June 14:30


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









#### Update Friday 19th June 2020 13:00

Over the last four weeks our system team have been working alongside the HPE team and have made excellent progress with the rebuilding of Cirrus. We expect Cirrus to be available for internal and some external user testing on Monday 22nd June.

The HPE team are now able to visit the Advanced Computing Facility (ACF) next Tuesday and Wednesday to complete the physical installation of the new GPU nodes.

We anticipate that the full Cirrus Service will be available to all users from Thursday 25th June.

Cirrus users will be required to use two credentials to access the service: an SSH key with a passphrase and their Cirrus password. It is imperative that users do not reuse a previously used password or SSH key with passphrase. All users will be asked to verify their SAFE accounts and we request that academic users use their UK home institutional email address for their SAFE account. If you are an academic user, who does not have a UK academic email address (.ac.uk), then we will require confirmation from your PI that you are an active collaborator within the project before we can add you to the access list. Industrial customers will be added to the access list.

New documentation which details how to log on with the new access arrangements will be provided.

Please also contact the Cirrus Service Desk if you have any concerns regarding this and apologies for the inconvenience caused.
 

#### Update Friday 22nd May 2020 1800

We appreciate your patience with the unavailability of Cirrus at the current time.
We continue to work with HPE to develop a plan to return a secure service to operation as soon as possible to enable your research to continue.
 
We anticipate that Cirrus will be returned to service on Monday 22nd June.
 
We do apologise for this unplanned downtime and acknowledge that it may be longer than you wish, however we believe taking the additional time now will return a more secure and better managed system going forward. It will also allow HPE time to complete the installation of Cirrus Phase II. We will adjust project duration to account for this downtime. 
 
As you may be aware EPCC were successful in the Tier 2 HPC call to fund Cirrus Phase II. The Cirrus Phase II service will build on the success of the Cirrus service by adding additional tightly integrated GPU accelerators to the system.
GPU accelerators help supercomputing applications run faster by accelerating their core numerical calculations.
 
Cirrus Phase II will have 144 NVIDIA V100 GPUs in addition to the 8 Cirrus already has and it is supported by a fast storage layer for data intensive applications.
 
Further updates will be provided by user mailings and please continue to check the Cirrus status page: http://www.cirrus.ac.uk/status/
Please also contact the Cirrus Service Desk if you have any concerns regarding this and apologies for the inconvenience caused.
 

#### Update Tuesday 19th May 2020 1100

We want to provide an update on the security incident on the Cirrus service. 
The Cirrus System Team continues to work on Cirrus and are in discussions with HPE regarding the return to service plan. 
We appreciate your understanding during this period of disruption. If you have any particular questions or concerns please get in touch via the service desk.


#### Update Friday 15th May 2020 1600

We want to provide an update on the security incident on the Cirrus service. 
EPCC and HPE are continuing to work analysing Cirrus to better understand the position and plan effective remedies. Our current investigation suggests that user data has not been taken or compromised. 
While our investigations continue, Cirrus will be unavailable and we apologise for the inconvenience caused by this outage. 
We appreciate your understanding during this period of disruption and a further update will be provided on Monday 18th May. If you have any particular questions or concerns please get in touch via the service desk.


#### Update Thursday 14th May 2020 1900

We wanted to take the time to provide an additional update on the identified security exploit that has been identified on the Cirrus service. 
It has become clear that this issue is something which is affecting a number of UK, European and International sites and systems, with Cirrus being one.
 
EPCC are continuing to work analysing Cirrus and working with HPE to better understand the position and plan effective remedies. Our current investigation suggests that user data has not been taken or compromised.
While our investigations continue, Cirrus will be unavailable and we apologise for the inconvenience caused by this outage. 

We appreciate your understanding during this period of disruption and a further update will be provided tomorrow.


#### Update Wednesday 13th May 2020

We wanted to take the time to provide an update on the identified security exploit that has been identified on the Cirrus service.

Over the last 24 hours, EPCC has been in contact with relevant parties within the University of Edinburgh, vendors and Government bodies, including the National Cyber Security Centre (NCSC) in order to construct the timeline of the exploit. This work is vital in order to help us understand where this exploit originated from, first sight of this exploit being on our services and any potential malicious activity on our services.

At this time, EPCC has been continuing to work analysing our other services as this is not a OS or unique service specific exploit and other services can be affected.

While we continue to conduct our investigations and work closely with NCSC to develop a wider understanding, Cirrus will be unavailable.

Additionally, EPCC are at this moment working on planned work that is required to return to service and this discussion is moving forward so that we can be as clear as possible of what is required in order to reduce the risk as much as possible this exploit reoccurring. At this stage we cannot provide any updates on potential return to service dates but will share this information as soon as this is available through our discussions with NCSC and other vendors.

We appreciate your understanding during this period of disruption. A further update will be provided later this afternoon. 

#### Tuesday 12th May 2020

Cirrus will be unavailable today, Tuesday 12th May 2020,  as we continue to investigate the security incident that was discovered yesterday.  Jobs that are currently running or queued will continue to run, but you will be unable to log in or to submit new jobs.  We will bring Cirrus back into service as soon as is safely possible to minimise disruption to the user community.  We hope to be in a position by tomorrow to provide a clearer idea of timescales for service resumption  and will provide a further update tomorrow.

We appologise for the inconvenience caused.  If you have any particular questions or concerns please get in touch via the service desk.

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





