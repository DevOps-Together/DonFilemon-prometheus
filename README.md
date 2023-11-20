# DonFilemon-prometheus

Napisz playbook + role Ansible instalujacy prometheus + node-exporter + grafana

## Zalozenie

kazdy komponent powinien znajdowac sie na innym hoscie najelpiej maszynie VM,
maszyny powinny znajdowac sie we wspolnej podsieci czyli 3 hosty

* jeden dla Prometheusa
* drugi dla Node-exporter
* trzeci dla Grafany

dodatkowo kazdy komponent powinien byc osobna rola, playbook ma odpalac role i zawierac vars

## Setup

### Setup Ansible

1. `cd ansible`
2. (setup once) `virtualenv -p python3 .ansible_env`
3. `source .ansible_env/bin/activate`
4. (setup once) `pip3 install -r requirements.txt`

### Setup vms using vagrant

1. `cd vagrant`
2. `vagrant up`

## Cleanup

### Delete vms using vagrant

1. `cd vagrant`
2. `vagrant destroy -f`

### Delete Ansible virtualenv

1. `rm -r .ansible_env`
