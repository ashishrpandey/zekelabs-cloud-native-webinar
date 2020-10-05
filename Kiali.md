# Kiali

Grafana is open source visualization and analytics software tool to turn your time-series database (TSDB) data into beautiful graphs and visualizations.
It allows you to query, visualize, alert on, and explore your metrics no matter where they are stored.

## Kiali Dashboard

- When Istio runs with "Demo" profile, it is enabled to run with Kiali.
- If you are running with Default profile, make sure you enable Kiali in the Istio-Operator yaml file.
- Get the list of all services running in istio-system name space

        kubectl get svc -n istio-system | grep -i kiali
    
- Edit kiali service to make its type NodePort
- Find out the randomly assigned NodePort of Kiali service

- Open in Borwser the following address 

        http://public-ip:NodePort/
        
- Default username and password both is admin 
        
- Generate some traffic by clicking multiple times on the demo-web application, and look at the graph created by Kiali to exactly see the traffic in green. 

