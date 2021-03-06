---
title: Components
type: Details
---

Kyma is built on the foundation of the best and most advanced open-source projects which make up the components readily available for customers to use.
This section describes the Kyma components.

## Service Catalog

The Service Catalog lists all of the services available to Kyma users through the registered Service Brokers. Using the Service Catalog, you can provision new services in the
Kyma [Kubernetes](https://kubernetes.io/) cluster and create bindings between the provisioned service and an application.

## Service Brokers

Service Brokers are [Open Service Broker API](https://www.openservicebrokerapi.org/)-compatible servers that manage the lifecycle of one or more services. Each Service Broker registered in Kyma presents the services it offers to the Service Catalog. You can provision these services on a cluster level through the Service Catalog. Out of the box, Kyma comes with three Service Brokers.
You can register more [Open Service Broker API](https://www.openservicebrokerapi.org/)-compatible Service Brokers in Kyma and provision the services they offer using the Service Catalog.

## Application Connector

The Application Connector is a proprietary Kyma solution. This endpoint is the Kyma side of the connection between Kyma and the external solutions. The Application Connector allows you to register the APIs and the Event Catalog, which lists all of the available events, of the connected solution. Additionally, the Application Connector proxies the calls from Kyma to external APIs in a secure way.

## Event Bus

Kyma Event Bus receives Events from external solutions and triggers the business logic created with lambda functions and services in Kyma. The Event Bus is based on the [NATS Streaming](https://nats.io/) open source messaging system for cloud-native applications.

## Service Mesh

The Service Mesh is an infrastructure layer that handles service-to-service communication, proxying, service discovery, traceability, and security independent of the code of the services. Kyma uses the [Istio](https://istio.io/) Service Mesh that enforces RBAC (Role Based Access Control) in the cluster. [Dex](https://github.com/coreos/dex) handles the identity management and identity provider integration. It allows you to integrate any [OpenID Connect](https://openid.net/connect/)-compliant identity provider with Kyma.   

## Serverless

The Kyma Serverless component allows you to reduce the implementation and operation effort of an application to the absolute minimum. Kyma Serverless provides a platform to run lightweight functions in a cost-efficient and scalable way using JavaScript and Node.js. Kyma Serverless is built on the [Kubeless](http://kubeless.io/) framework, which allows you to deploy lambda functions,
and uses the [NATS](https://nats.io/) messaging system that monitors business events and triggers functions accordingly.  

## Monitoring

Kyma comes bundled with tools that give you the most accurate and up-to-date monitoring data.  [Prometheus](https://prometheus.io/) open source monitoring and alerting toolkit provides this data, which is consumed by different add-ons, including [Grafana](https://grafana.com/) for analytics and monitoring, and [Alertmanager](https://prometheus.io/docs/alerting/alertmanager/) for handling alerts.

## Tracing

The tracing in Kyma uses the [Jaeger](https://github.com/jaegertracing) distributed tracing system. Use it to analyze performance by scrutinizing the path of the requests sent to and from your service. This information helps you optimize the latency and performance of your solution.

## Logging

Logging in Kyma uses [Logspout](https://github.com/gliderlabs/logspout) and [OK Log](https://github.com/oklog/oklog). Use a plaintext or a regular expression to fetch logs from pods using the OK Log UI.
