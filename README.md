Welcome to StarVE !
===================

### 目录



[TOC]



Iterface Document
-------------


----------


----------


#### <i class="icon-file"></i> Base
***
##### **1.  function set_firewall()**
接口名称：set_firewall
接口描述：
输入参数：	**None**			
输出结果：
&emsp;**Status:**
&emsp; &emsp;**0     success**
&emsp; &emsp;**1     failed**

***
##### **2. function set_selinux()**
接口名称：set_selinux
接口描述：
输入参数：	**None**			
输出结果：
&emsp;**Status:**
&emsp; &emsp;**0     success**
&emsp; &emsp;**1     failed**

***
##### **3. function set_hostname()**
接口名称：set_hostname
接口描述：
输入参数：	**hostname**	**ipaddr**		
&emsp;示例：
&emsp;&emsp;hostname=test01  
&emsp;&emsp;ipaddr=10.6.0.111   
&emsp;&emsp;set_hostname   \$hostname    \$ipaddr
&emsp;&emsp;ret=$?
输出结果：
&emsp;**Status:**
&emsp; &emsp;**0     success**
&emsp; &emsp;**1     failed**


***
##### **4. function check_remote_host()**
接口名称：check_remote_host
接口描述：
输入参数：	**remote**	
&emsp;示例：
&emsp;&emsp;remote=10.6.0.115
&emsp;&emsp;check_remote_host  \$remote
&emsp;&emsp;ret=$?
输出结果：
&emsp;**Status:**
&emsp; &emsp;**0     success**
&emsp; &emsp;**1     failed**

***
##### **5. function set_timesync()**
接口名称：check_remote_host
接口描述：
输入参数：	**iplist**	(time sync server ip list)
&emsp;示例：
&emsp;&emsp;iplist=(1.1.1.1  2.2.2.2  3.3.3.3  4.4.4.4)
&emsp;&emsp;set_timesync \${iplist[@]}
&emsp;&emsp;ret=$?
输出结果：
&emsp;**Status:**
&emsp; &emsp;**0     success**
&emsp; &emsp;**1     failed**

***
##### **6. function get_nic_name()**
接口名称：get_nic_name
接口描述：
输入参数：	None
&emsp;示例：
&emsp;&emsp;ifaces=()
&emsp;&emsp;ifaces=$(get_nic_name)
输出结果：
&emsp;**niclist:**(net interface list,an array)

***
##### **7. function set_nic_with_bridge()**
接口名称：set_nic_with_bridge
接口描述：
输入参数：	
&emsp;**NIC**	 (网卡名)
&emsp;**br** (桥接名)
示例：
&emsp;&emsp;nic=eth0
&emsp;&emsp;br=br0
&emsp;&emsp;set_nic_with_bridge \$nic \$br
&emsp;&emsp;ret=$?
输出结果：
&emsp;**Status:**
&emsp; &emsp;**0     success**
&emsp; &emsp;**1     failed**

***
##### **8. function set_bridge()**
接口名称：set_bridge
接口描述：
输入参数：	
&emsp;**br**	 (桥接名)
&emsp;**ip** (网桥IP)
&emsp;**netmask** (网桥掩码)
&emsp;**gateway** (网桥网关)
示例：
&emsp;&emsp;br=br0
&emsp;&emsp;ip=192.168.0.101
&emsp;&emsp;netmask=255.255.255.0
&emsp;&emsp;gateway=192.168.0.1
&emsp;&emsp;set_bridge \$br \$ip \$netmask \$gateway
&emsp;&emsp;ret=$?
输出结果：
&emsp;**Status:**
&emsp; &emsp;**0     success**
&emsp; &emsp;**1     failed**

***
##### **9. function set_nic_with_bond()**
接口名称：set_nic_with_bond
接口描述：
输入参数：	
&emsp;**NIC**	 (网卡名)
&emsp;**bond** (绑定名称)
示例：
&emsp;&emsp;nic=eth0
&emsp;&emsp;bond=bond0
&emsp;&emsp;set_nic_with_bond \$nic \$bond
&emsp;&emsp;ret=$?
输出结果：
&emsp;**Status:**
&emsp; &emsp;**0     success**
&emsp; &emsp;**1     failed**

***
##### **10. function set_bond()**
接口名称：set_bond
接口描述：
输入参数：	
&emsp;**bond**	 
&emsp;**niclist**
&emsp;**br** 
示例：
&emsp;&emsp;bond=bond0
&emsp;&emsp;niclist=(eth0 eth1 eth2 eth3)
&emsp;&emsp;br=br0
&emsp;&emsp;set_bond \$bond \${niclist[@]} \$br
&emsp;&emsp;ret=$?
输出结果：
&emsp;**Status:**
&emsp; &emsp;**0     success**
&emsp; &emsp;**1     failed**

***
##### **11. function set_multipath()**
接口名称：set_bond
接口描述：
输入参数：	None 
示例：
&emsp;&emsp;set_multipath
&emsp;&emsp;ret=$?
输出结果：
&emsp;**Status:**
&emsp; &emsp;**0     success**
&emsp; &emsp;**1     failed**


----------


----------


#### <i class="icon-file"></i> NFS Server



#### <i class="icon-file"></i> Server



#### <i class="icon-file"></i> Agent-HA ( High Availability )




#### <i class="icon-file"></i> Agent-TP ( Thin Provisioning )



> **Tip:** 


----------






