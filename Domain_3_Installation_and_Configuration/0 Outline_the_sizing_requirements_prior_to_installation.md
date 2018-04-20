# Outline the sizing requirements prior to installation

## Official Docker Documentation
[Hardware and software requirements](https://docs.docker.com/datacenter/ucp/2.2/guides/admin/install/system-requirements/#hardware-and-software-requirements)  
Docker EE
Linux 3.10+
Static IP

Minimum Managers need 8 but workers need 4 but all get 3Gb of disk space
Recommended 16GB with 4 vCPU and 25-100GB of space.
Assumptions is that managers do not carry workloads if they do add some Space. 

[DTR requirements](https://success.docker.com/KBase/What_are_the_minimum_requirements_for_Docker_Trusted_Registry_(DTR)%3F)  
Come with notary
provides signing and audit capabilites
cleans up after itself. 

[Docker EE best practices and design considerations](https://success.docker.com/article/Docker_Reference_Architecture-_Docker_EE_Best_Practices_and_Design_Considerations_17_03)  
4GB Ram
3GB disk space

A maintained version of CentOS 7. Archived versions aren’t supported or tested.
Red Hat Enterprise Linux 7.0, 7.1, 7.2, or 7.3
Ubuntu 14.04 LTS or 16.04 LTS
SUSE Linux Enterprise 12
Oracle Linux 7.3

