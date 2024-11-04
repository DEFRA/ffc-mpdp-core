# Making Payment Data Public Core
Local development support for orchestrating all MPDP microservices

## Prerequisites

Ensure you have satisfied the prerequisites of all individual repositories.

## Repositories
- [ffc-mpdp-frontend](https://github.com/DEFRA/ffc-mpdp-frontend)
- [ffc-mpdp-backend](https://github.com/DEFRA/ffc-mpdp-backend)

## Scripts

### Clone

Clone all repositories from GitHub.  Repositories will cloned in the parent directory of this repository.

[`./clone`](clone)

### Update

Switch to `main` branch in every repository and pull latest changes with `git pull`.

[`./update`](update)

### Build

Build/rebuild Docker container for all microservices.

[`./build`](build)

### Start

Run all services.

[`./start`](start)

#### Optional arguments

Any valid `docker-compose down` argument.


### Stop

Stop all services.

[`./stop`](stop)

#### Optional arguments

Any valid `docker-compose down` argument.

### Open

Open all services in Visual Studio Code.

[`./open`](open)

### Latest versions

List latest GitHub release version for each microservice.

[`./latest-versions`](latest-versions)

### Environment versions

List current environment version for each microservice hosted in Kubernetes.

[`./environment-versions`](environment-versions)

#### Options
- `-c | --cluster` - Kubernetes cluster context name
- `-n | --namespace` - Kubernetes namespace

### Resource quota

Determine the Kubernetes resource usage for a namespace based on all microservices running at maximum capacity and scaling.

[`./resource-quota`](resource-quota)
