# random-inspirational-messages-kubernetes

🚧 Still working in progress.

POC to deploy dockerized application to EKS.

### Backend

Providing random inspirational messages from `/message` endpoint.

You can see backend application [here](https://github.com/setkyar/random-inspirational-messages-be)

### Frontend

Getting random inspirational messages from backend endpoint and disply them via UI.

You can see frontend application [here](https://github.com/setkyar/random-inspirational-messages-fe)


## Usage

First you have to create eks cluster with nodegroups. After that you can deploy.


### Create cluster

You can check [here](./eksctl/README.md) for instruction.


### Deploy Kubernetes

#### Deploy backend

First, you have to deploy backend. Since it's required backend API endpoint.

You can check the detail inside the [backend folder](./backend/README.md).

#### Deploy frontend

After finishing up the backend, you have to get backend URL and update your frontend `index.html` page for correct domain. Then push docker and update `deployment.yaml` file to use correct version of the docker build.

After that, you should be able to deploy. For the deployment you can check the [frontend folder](./frontend/README.md) for detail.