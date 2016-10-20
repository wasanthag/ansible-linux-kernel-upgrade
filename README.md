# ansible-linux-kernel-upgrade
ansible playbook to manually compile and install new kernel on Centos/Redhat Linux

```
Script needs an inventory file when run against real servers.
For local testing with vagrant use hosts: all
For silent kernel compile, a kernel config file with required kernel configs options is required. This can be obtained by manually compiling
the kernel on one of the hosts. Kernel confg file .config can be found inside the folder where the kernel is compiled. 
This playbook expect the kernel config file (kernel.config) file to be in the same folder as playbook upgrade.yml.
A sample kernel config with default options are included in the script folder.
syntax to run the script is ansible-playbook upgrade.yml -i inventory.yml -u root -k
This is tested with ansible 2.0
```

