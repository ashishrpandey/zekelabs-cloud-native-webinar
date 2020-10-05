# Grafana

Grafana is open source visualization and analytics software tool to turn your time-series database (TSDB) data into beautiful graphs and visualizations.
It allows you to query, visualize, alert on, and explore your metrics no matter where they are stored.

## Grafana Dashboard

- When Istio runs with "Demo" profile, it is enabled to run with Grafana.
- If you are running with Default profile, make sure you enable Grafana in the Istio-Operator yaml file.
- Get the list of all services running in istio-system name space

        kubectl get svc -n istio-system | grep -i grafana
    
- Edit grafana service to make its type NodePort
- Find out the randomly assigned NodePort of grafana service

- Open in Borwser the following address 

        http://public-ip:NodePort/
        
- Import Dashboard with Id 11141 to see the "Analysis by Pod" dashboard
