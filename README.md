# otel-python-k8s

Using otel on python at k8s env

Apply it to the cluster
```
kubectl apply -k .
```

Use port-forward to acess tracing
```
kubectl port-forward --address 0.0.0.0 services/tracing 16686:16686 16685:16685 -n default
```

# Rereferences

* [OpenTelemetry/Operator Repo](https://github.com/open-telemetry/opentelemetry-operator)

* [OpenTelemetry Patterns](https://github.com/jpkrohling/opentelemetry-collector-deployment-patterns)

* [IsItObservable Video](https://www.youtube.com/watch?v=tuiPSfqrmtg)

* [IsItObervable Repo](https://github.com/isItObservable/OpenTelemetryOperator)