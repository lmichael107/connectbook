
[title]: - "Guidelines for data managment in OSG - Storage and Transfer"

## Purpose

The following tables provide the guidelines of data management in OSG. Check the web link for details. 


## Data Storage

|         | Recommended Limit| Purpose | Details|
| ------- |:----------------:| :------:| ------:|
| home    | 0-5 GB      | Meant for quick data access and not for submitting jobs.| [Data Storage](https://support.opensciencegrid.org/support/solutions/articles/12000002985-storage-solutions-on-osg-home-stash-and-public)|
| stash   |  < 1 TB GB  | Meant for large storage and I/O of your jobs. |[Data Storage](https://support.opensciencegrid.org/support/solutions/articles/12000002985-storage-solutions-on-osg-home-stash-and-public)|
| public  |  < 10 GB    | Meant for sharing data and input data  transfer via HTTP|[Data Storage](https://support.opensciencegrid.org/support/solutions/articles/12000002985-storage-solutions-on-osg-home-stash-and-public)|



## Input data for your job

|    Protocol     | Data Size| command| Purpose | Details|
| --------------- |:----------:| :-----:|:--------|--------:|
| HTCondor    | < 1 GB       | transfer_input_files| Input data from home, public or stash |[HTCondor Transfer](https://support.opensciencegrid.org/support/solutions/articles/5000639787-transferring-data-with-htcondor)|
| HTTP        |  < 10 GB   | wget, curl or transfer_input_files  | Input data from ~/public |[HTTP Access](https://support.opensciencegrid.org/support/solutions/articles/5000639798-access-stash-remotely-using-http)|
| StachCache  |  < 50 GB    | Staschcp |Input data from ~/public| [StachCache](https://support.opensciencegrid.org/support/solutions/articles/5000639798-access-stash-remotely-using-http)|


## Output data for your job
The solutions for data transfers from your job back to OSG Connect are more limited. At this point, we recommend that you use the built-in HTCondor file transfer mechanism (transfer_output_files=... in your job submit file).


## External data transfer

|    Protocol | Data Size| Details|
| ------------|:--------:| ------:|
| scp         | < 1 GB   | [SCP](https://support.opensciencegrid.org/support/solutions/articles/5000634376-using-scp-to-transfer-files) |
| Globus      |  > 1 GB  | [Globus](https://support.opensciencegrid.org/support/solutions/articles/5000632397-data-transfer-with-globus) |


## Getting Help
For assistance or questions, please email the OSG User Support team  at [user-support@opensciencegrid.org](mailto:user-support@opensciencegrid.org) or visit the [help desk and community forums](http://support.opensciencegrid.org).

