- `git clone https://github.com/CentOS-PaaS-SIG/linchpin.git`
- `cd linchpin`
- `curl -L -4 https://github.com/CentOS-PaaS-SIG/linchpin/pull/1009.diff | patch -d . -p1`
- `virtualenv --python=/usr/bin/python2.7 .venv; source .venv/bin/activate`
- `pip install -v . python-openstackclient`
- `./scripts/install_selinux_venv.sh`
- `linchpin init rhhi`
- `cd rhhi`
- `git clone https://github.com/mcornea/metalkube-dev-scripts-openstack.git .`
- `## set credentials in hooks/ansible/post/extravars.yml`
- `./deploy.sh`

![alt text](https://raw.githubusercontent.com/mcornea/metalkube-dev-scripts-openstack/master/rhhi-openstack.png)
