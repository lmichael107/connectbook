[title]: - "OSG Managed Services"

## How the Service Works

OSG offers a *managed service option* to connect a campus HPC/HTC cluster to the Open Science Grid. The OSG team will host and operate an HTCondor compute element which routes user jobs to your cluster, configured for science communities that you choose to support. 

![fig bosco](https://raw.githubusercontent.com/OSGConnect/connectbook/master/images/screenshot_2980.png)


## Requirements

Here are the basic system requirements:

* Cluster operating system must be CentOS 6.x, 7.x or Scientific Linux 6.x, 7.x 
* A standard Unix account on your system's login server. The OSG service will use this account and submit to your batch queue in a manner you define.
* SSH access to this account via public SSH keys.
* A supported batch system (Slurm, HTCondor, PBS, LSF, SGE)

## Setup Process

Setup and installation process consists of the following steps:
  
* Consultation call to collect system details
* Create Unix login account for the OSG service
* Install public SSH keys for the service
* We configure the OSG service with your system details
* We validate operation with a set of test jobs
* We configure central OSG services to schedule jobs for science communities you support
* (Optional): we can assist you in installing and setting up the Squid and OASIS software on your cluster 

## Which Science Communities and Institutions am I supporting?

The OSG provides monitoring to view which communities are accessing your site, their fields of science, home institution. Below is an example of the monitoring views that will be available for your cluster. 

![fig gracc](https://raw.githubusercontent.com/OSGConnect/connectbook/master/images/screenshot_2979.png)


## Optional: Providing Access to Application Software Using OASIS

Many OSG communities use software modules provided by their collaborations or by the OSG User Support team. You do not need to install any application software on your cluster. OSG uses a FUSE-based distributed software repository system called OASIS. To support these communities, the following additional components are needed: 
       
* A (cluster-wide) Squid service with a minimum 50GB of cache space.
* Local scratch area on compute nodes: typical recommendations are 20 GB per job
* On each compute node, installation of the OASIS software package and associated FUSE kernel modules
* Local scratch space of 5 GB.

### Install the OSG Packaged Squid Service

The OSG Squid service comes preconfigured to point to certified OSG software repositories.  Instructions, or pointer to..

### Install the OSG OASIS Software on Your Cluster Compute Servers

Instructions...or pointer to.

## Getting Started

Drop us a note at [user-support@opensciencegrid.org](mailto:user-support@opensciencegrid.org) if this is of interest to you. We will contact you to setup a consultation.  