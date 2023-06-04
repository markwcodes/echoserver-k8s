# echoserver-k8s
#### A simple Echo server for testing Kubernetes ingress

Live demo: [echo.wilson.codes](https://echo.wilson.codes)\
(_Refresh a few times and see the load balancer connecting you to different pod replicas!_)

## About

This echo server deployment provides a simple way to test your public ingress in any Kubernetes cluster.

The deployment echoes the request header data from your browser back at you, thus allowing you to test reachability from outside as a public user.

## Setup

1. Install the cert-manager CRDs and resources following [this guide](https://cert-manager.io/docs/installation/).
2. Enter your DigitalOcean access key in `do-secret.yml`
3. Deploy with `kubectl -n echo-server apply -f .`
