---
description: Overview of GKO.
---

# GKO 4.9

## Highlights

Gravitee Kubernetes Operator (GKO) 4.9 introduces several key improvements focused on enhanced configuration, better support for notifications, and simplified troubleshooting.

## Product

### New Features

#### Helm Chart configuration

The GKO 4.9 Helm Chart offers new customization options for the operator manager pod's deployment. You can now set node selectors to control where the pod is scheduled, apply common annotations and labels to all Helm release components, configure an HTTP proxy for the operator manager's internal client, and set a security context on the deployment.

#### Notification enhancements

The Notification Custom Resource now supports groups created directly within the Gravitee API Management (APIM) Console, as opposed to only those created through a Group Custom Resource. This new feature allows the `groups` attribute within a Notification Custom Resource to reference these Console-defined groups.

#### Simplified troubleshooting

GKO 4.9 simplifies troubleshooting by using resource status conditions to reflect reconciliation errors. This new feature provides a more transparent view of the resource's state without requiring users to dive into the operator manager's logs. When a resource encounters a problem, its status conditions provide direct feedback, making it easier to identify and fix issues.

## Deprecation notice

`processingStatus` is being deprecated in favor of conditions for custom resource statuses.
