### Installing Monitoring with Prometheus, Grafana, Node_exporter

1). Create domain for Prometheus, Grafana
    - example : `prometheus.<your_domain_name>.com`, `grafana.<your_domain_name>.com`

2). Edit some valuse on ansible path with line `<some_values>`
    - ansible/hosts.init
    - ansible/monitoring/defaults/main.yml
    - ansible/monitoring/templates/prometheus.yml

3). After already installed for grafana,prometheus servers, Step adding "datasource" On grafana using `prometheus.<your_domain_name>.com` without "port"
    * Cause used Nginx reverse proxy to docker container