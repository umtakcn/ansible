Redis Cluster and Sentinel Playbook with Stunnel Option.

You can install Redis Cluster or Sentinel with or without Stunnel via this Ansible role.

Once you start the role, you will be asked to choose from Redis Cluster or Sentinel. After you select it, again you will be asked whether you want Stunnel or not.

If you select Cluster, role will create three node six instance Redis Cluster. If you select Sentinel, role will create three node Sentinel.

Two thing you need to do before run this role. First you need to specify three server ip (1 Master, 2 Slave) in inventory file. Second, you need to place Redis setup file in /opt/files on Ansible server and rename its name to "redis". If you select Stunnel too, you need to set certificate too which is under tasks/stunnel. You can also change redis configuration file variables. All variables are under vars folder.
