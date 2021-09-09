Role Name
=========
ansible-atop-redhat

Description
---------------
Ansible role to configure the atop diagnostic tool on Red Hat Linux systems.

This role was developed and tested on a Mint 20.2 system using [Molecule 3](https://molecule.readthedocs.io/en/latest/) with the Docker driver and Red Hat 7 and 8 containers from [Red Hat's Container Registry](https://catalog.redhat.com/software/containers/explore). A simple Dockerfile and configuration are included.

Molecule 3 changed the default verifier to Ansible (from testinfra). A basic test setup for Molecule 3 is included as well.

Full instructions for setting up this environment are a available at [GeoffStratton.com](http://www.geoffstratton.com/test-ansible-roles-molecule-3-and-red-hat-docker-images-linux-mint).

To use official RHEL images you'll need to generate a Red Hat Container Registry [service account](https://access.redhat.com/terms-based-registry/). (Yes, you can do with this with the free Red Hat Developer subscription.) You'll then need to provide your username and password token to the molecule.yml file; I just used shell variables but you could also use a CI/CD tool or other methods.

Requirements
--------------
* ansible
* molecule
* python

License
-------
GNU General Public License v3.0

Author Information
------------------
Geoff Stratton
