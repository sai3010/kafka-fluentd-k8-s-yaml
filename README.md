# kafka-fluentd-k8-s-yaml
- Kubernetes yaml files to run fluentd-kafka collector on k8's to collect container logs and push to kafa topic

- Refer to [kafka-fluentd-docker](https://github.com/sai3010/kafka-fluentd-docker/) to build a docker and run it using this yaml file.

# Note 
- Modify the fluentd-config file by referring to [kafka-plugin](https://github.com/fluent/fluent-plugin-kafka)

# Deploying fluentd as daemon set on k8's
- ```kubectl create namespace logging```
- ```kubectl apply -f fluentd-config.yaml```
- ```kubectl apply -f fluentd-config.yaml```

## TO-DO
- Accept kafka parameters from env