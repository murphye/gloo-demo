# Advancecd Gloo Demo

This demo script assumes the following are already set up. Specific installation instructions are documentated separately. This repository focuses on the demo script itself.

1. 3 separate Kubernetes clusters (examples use Google Cloud)
2. Gloo Edge installed on 2 clusters
3. Gloo Edge Federation installed on 1 management cluster
4. Argo installed on 2 clusters
5. Appropriate command line tools installed (kubectl, glooctl, helm)

##  Scenario

* A Todo application, written in Java, has a simple UI interface, and a REST interface for adding and removing Todos.

### Scenario Part 1

* There is an OpenAPI spec that is deployed with the application at the `/openapi` endpoint.
* The hosted UI for the application should have free access to the API endpoints.
* External consumers of the application should only have access with an API key, via a Gloo API Product.

### Scenario Part 2

* 

