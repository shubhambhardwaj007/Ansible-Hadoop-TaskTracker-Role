<a href="https://hadoop.apache.org/"><img src="images/Hadoop_logo.svg" width="100%" height="100%"></a>

# Ansible-Hadoop-TaskTrackerNode-Role

An Ansible Role to Configure and setup [Hadoop](https://hadoop.apache.org/) Task Tracker Node.

Requirements
------------
This role is dependent upon `shubhambhardwaj007.hadoop_software_setup`.
For a full usage example with the `shubhambhardwaj007.hadoop_software_setup` role, see the Example Playbook later in this README.

Role Variables
--------------
Available variables are listed below, along with default values (see vars/main.yml):
```
Job_Tracker_Mapreduce_Port: "9002"
```
The `Job_Tracker_Mapreduce_Port` should be similar to exposed port by Hadoop Job Tracker Node.

Dependencies
------------
None

Example Playbook
----------------
```
 - hosts: tasktracker_node
   roles:
     - shubhambhardwaj007.hadoop_software_setup
     - shubhambhardwaj007.hadoop_tasktracker
```
License
-------

GNU

Author Information
------------------
This role was created in 2021 by [Shubham Bhardwaj](https://galaxy.ansible.com/shubhambhardwaj007/hadoop_tasktracker)
