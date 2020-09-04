# Roadmap & Accomplishments

## Alpha-Testing Phase

_Starting September 1, 2020_  

* [x] Invite self-sufficient, advanced HPC users to try out the C4 cluster and to give constructive feedback.

* [x] Scheduler: Rudimentary Slurm configuration with one shared partition ("queue") and one lab-owned partition.

   - [x] Interactive jobs, e.g. `srun --pty bash`.

* [x] c4-help issue tracker <https://github.com/UCSF-CBI/c4-help>

* [x] Shared CBI software + modules, i.e. /software/c4/CBI/

* [ ] Shared software + modules of other labs: /software/c4/<group>/

* [ ] Website: Set up a C4 website with the most basic documentation.

* [ ] Lab compute nodes: 4 new lab nodes (4*56 = 224 physical cores).

* [ ] Mount lab storage: ... (three labs)

* [ ] Add one communal node (TIPCC node n2)


## Beta-Testing Phase

* [ ] Invite more advanced single-node labs (e.g. Francis Lab)

* [ ] Some more EPEL package requests (probably not much)

* [ ] Slurm well documented + Torque-to-Slurm translation table

* [ ] Password aging

* [ ] LDAP?


## Migration

We know everything works fine. No going back.

* [ ] c4-announce mailing list

* [ ] Only allow active accounts with up-to-date contact information (and keeping it up-to-date)

* [ ] All TIPCC should start migration to C4

* [ ] ...



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
