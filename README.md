# Zabbix-Linux-Disk-Performance-Template
Template to autodiscovery disks and collect performance statistics


Administration -> General -> Regular expressions -> New regular expression

Name: Linux disks for autodiscovery

Expressions
  EXPRESSION TYPE: Result is TRUE
  EXPRESSION: ^(hd[a-z]+|sd[a-z]+|xvd[a-z]+|vd[a-z]+|dm-[0-9]+|drbd[0-9]+|nvme[0-9]+n[0-9]+)$

  EXPRESSION TYPE: Result is FALSE
  EXPRESSION: ^(vzsnap.*|.*-cow|.*-real|ram[0-9]+|loop[0-9]+|sr[0-9]*|fd[0-9]*)$
