# Jaeger 

Jaeger is open source software for tracing transactions between distributed services. It’s used for monitoring and troubleshooting complex microservices environments.
Jaeger provides - 
- Distributed context propagation
- Distributed transaction monitoring
- Root cause analysis
- Service dependency analysis
- Performance / latency optimization

## Jaeger Dashboard

- When Istio runs with "Demo" profile, it is enabled to run with Istio-tracing.
- Get the list of all services running in istio-system name space

        kubectl get svc -n istio-system | grep -i jaeger
    
- Edit jaeger query service to make its type NodePort
- Find out the randomly assigned NodePort of jaeger service

- Open in Borwser the following address 

        http://public-ip:NodePort/
        

