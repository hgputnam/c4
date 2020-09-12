# Roadmap & Accomplishments

## Alpha-Testing Phase

_Starting September 1, 2020_  

**Who**: In this phase we're inviting self-sufficient, advanced HPC users to try out the C4 cluster and to give constructive feedback.

**What**: We will implement essential features that we missed previously.  We will address feature requests that are straightforward to implement.  More complex feature requests will be saved for later.

**Outcome**: At the end of this phase, we will have a rudimentary HPC environment that will allow advanced users to run scientific jobs.

### Scheduler

* [x] Rudimentary Slurm configuration with one shared partition ("queue") and one lab-owned partition.

* [x] Interactive jobs, e.g. `srun --pty bash`.

* [ ] Job email notification

* [x] Torque/PBS wrappers (emulating Torque/PBS on Slurm)

### Software

* [x] Shared CBI software + modules, i.e. /software/c4/CBI/

* [ ] Shared software + modules of other labs: /software/c4/{group}/

### Documentation and support

* [x] c4-help issue tracker <https://github.com/UCSF-CBI/c4-help>

* [ ] Set up a C4 website with the most basic documentation

* [ ] Tabular overview of the different host types available

### Compute power

* [x] Lab compute nodes: 4 new lab nodes (4*56 = 224 physical cores)

* [ ] Add another communal node (revive TIPCC node n2)

### Storage

* [ ] Mount _new_ lab storage (not available on TIPCC)

### Backup

* [x] Users' home directories are backed up

* [x] The software stacks under /software is backed up

### Miscellanous

* [ ] Idle shells with automatically log out after 24 hours

* [ ] All development and compute nodes have the same configuration of local /tmp and local /scratch


## Beta-Testing Phase

**Who**: Invite additional advanced users from other labs.  We are interesting in labs who are willing to migrate the exising TIPCC compute nodes over to C4, e.g. labs will a single compute node

**What**: Feature requests that were too complex for the alpha-testing phase will addressed.

**Outcome**: At the end of this phase, we will have a solid HPC environment that will allow the majority of users to run scientific jobs on C4 that they previously ran on TIPCC.  We are confident that we can go forward with inviting all TIPCC users.

### Scheduler

* [ ] Finalize basic configuration allowing users to submit as much as they want without starving out other users

* [ ] Add more lab-specific partitions

* [ ] All jobs are running through cgroup

### Documentation and support

* [ ] c4-announce mailing list

* [ ] Slurm well documented + Torque-to-Slurm translation table

* [ ] Common TIPCC-to-C4 migration issues and conflicts documented

### Software

* [ ] Some more EPEL package requests (probably not much)

* [ ] MATLAB using UCSF site-wide licenses

### Accounts

* [ ] Password aging

* [ ] Set up LDAP for account management

### Storage

* [ ] Mount _existing_ lab storage on TIPCC also on C4

### Miscellanous

* [ ] Expand existing Bash configuration to Csh


## Going Live

**Prerequisites**: We know everything works fine. No going back

**Who**: All TIPCC user are welcome to start using C4

### Accounts

* [ ] Users that migrate are added to LDAP.  Changes in LDAP will manually be mirrored on TIPCC

* [ ] Only allow active accounts with up-to-date contact information (and keeping it up-to-date)

### Software

* [ ] Very old, legacy scientific software on TIPCC will be re-installed on C4 if requested



## Migration

**Who**: All remaining TIPCC users who are not yet on C4

### Accounts

* [ ] All TIPCC users should start migration to C4

### Software

* [ ] We will attempt to accommodate legacy-software needs as far as possible



## TIPCC deprecation

* [ ] TIPCC is kept on life support only!

* [ ] TIPCC might crash at any time!




## Accomplished milestones

* Storage: Global scratch storage on BeeGFS parallel file system (2020-07-01)

* Login: 2 login nodes (June 2020)

* Development: Added two development nodes (2020-08-13)

* Compute nodes: 5 communal/common compute nodes (5*32=160 physical cores).

* Software: Replicate the core software that is installed on [Wynton HPC] on development and compute nodes (2020-08-19)

* Software: Added the CBI software stack (2020-08-20)

* Deployment of new machines: Automated deployment.

* Backup: Users' home accounts backed up on a nightly basis.

* Network: 10 Gbps.


See also [News].


[TIPCC]: https://ucsf-ti.github.io/tipcc-web/
[Wynton HPC]: https://wynton.ucsf.edu/hpc/
[BeeGFS]: https://www.beegfs.io/
[Globus]: https://www.globus.org/
[News]: {{ '/about/news.html' | relative_url }}
