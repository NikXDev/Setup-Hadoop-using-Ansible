# Setup-Hadoop-using-Ansible

In this task, we are configuring a Hadoop cluster service using Ansible Playbook.

<br>
1. What is Ansible?<br>
--> Ansible is an IT automation tool. It can configure systems, deploy software, and orchestrate more advanced IT tasks such as continuous deployments or zero downtime rolling updates. Ansible’s main goals are simplicity and ease-of-use. It also has a strong focus on security and reliability, featuring a minimum of moving parts, usage of OpenSSH for transport (with other transports and pull modes as alternatives), and a language that is designed around auditability by humans–even those not familiar with the program.

<br>
2. What is Hadoop?<br>
--> Apache Hadoop is an open source framework that is used to efficiently store and process large datasets ranging in size from gigabytes to petabytes of data. Instead of using one large computer to store and process the data, Hadoop allows clustering multiple computers to analyze massive datasets in parallel more quickly.

<br>
3. What are playbooks?<br>
--> An Ansible playbook is a blueprint of automation tasks—which are complex IT actions executed with limited or no human involvement. Ansible playbooks are executed on a set, group, or classification of hosts, which together make up an Ansible inventory. 

<br>
4. What is NameNode?<br>
--> NameNode is the master node in the Apache Hadoop HDFS Architecture that maintains and manages the blocks present on the DataNodes (slave nodes). NameNode is a very highly available server that manages the File System Namespace and controls access to files by clients.

<br>
5. What is DataNode?<br>
--> DataNodes are the slave nodes in HDFS. The actual data is stored on DataNodes. A functional filesystem has more than one DataNode, with data replicated across them. On startup, a DataNode connects to the NameNode; spinning until that service comes up.

<br>
Here, I'm launching a VM instance to get started with. All the playbooks and configuartion files are been set-up on this node. Execute the playbooks to get the task done. On successful set-up of hadoop cluster, run the following command to get the report of the cluster.
<br>

```
hadoop dfsadmin -report
```

Using the master's IP address, user can access the Hadoop WebUI.
```
# <master_IP>:<port_no>
192.168.1.13:50070
```

Configure and set-up the steps as described in the files and we are done.<br>
THANK YOU!
