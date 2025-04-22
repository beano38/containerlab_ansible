check and modify variables in the group_vars and host_vars directories

setup:

create python virtual environment
```python3.11 -m venv env```

activate virtual environment
```source env/bin/activate```

install python packages
```pip install -r requirements.txt```

install ansible collections
```ansible-galaxy install -r requirements.yml```

If you're running esxi environment for virtualization you can create the containerlab vm
```ansible-playbook deploy_vms.yml```

## Install Docker, Containerlab and containers
```ansible-playbook deploy_container_lab.yml```

make sure to check variables in the deploy_container_lab.yml playbook

you will need to get XRd images from cisco download site [Containerlab XRd page](https://containerlab.dev/manual/kinds/xrd/)
TODO, finish setting up TRex docker container