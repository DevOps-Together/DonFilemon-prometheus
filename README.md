# DonFilemon-prometheus
Napisz playbook + role Ansible instalujacy prometheus + node-exporter + grafana

# Zalorzenie 
kazdy komponent powinien znajdowac sie na innym hoscie najelpiej maszynie VM,
maszyny powinny znajdowac sie we wspolnej podsieci czyli 3 hosty
jeden dla Prometheusa
drugi dla Node-exporter
trzeci dla Grafany

dodatkowo kazdy komponent powinien byc osobna rola, playbook ma odpalac role i zawierac varsy

