# Prometheus 

An open-source monitoring system with a dimensional data model, flexible query language, efficient time series database and modern alerting approach.

## Prometheus Dashboard

- When Istio runs with "Demo" profile, it is enabled to run with prometheus.
- Get the list of all services running in istio-system name space

        kubectl get svc -n istio-system 
    
- Edit Prometheus service to make its type NodePort
- Find out the randomly assigned NodePort of Prometheus service

- Open in Borwser the following address 

        http://public-ip:NodePort/
        
        


