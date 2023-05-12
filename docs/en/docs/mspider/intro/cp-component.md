# Control plane components of the service mesh

| Component Name | Location | Description | Default Resource Settings |
| ---------------------------- | ------------ | ------- --------------------- | ---------------- |
| mspider-ui | Global Management Cluster | Service Mesh Interface | requests: CPU: Not set; Memory: Not set<br> limits: CPU: Not set; Memory: Not set |
| mspider-ckube | Global management cluster | Acceleration component of Kubernetes API Server, used to call global cluster-related resources | requests: CPU: not set; memory: not set<br/> limits: CPU: not set; memory: not set settings |
| mspider-ckube-remote | Global Management Cluster | Used to call Kubernetes of remote clusters, aggregate multi-cluster resources, and accelerate | requests: CPU: not set; memory: not set<br/> limits: CPU: not set; memory : not set |
| mspider-gsc-controller | Global management cluster | Service mesh management component, used for mesh creation, mesh configuration and other mesh control plane life cycle management, and Mspider control plane capabilities such as permission management | requests: CPU: Not set ;memory: not set<br/>limits: CPU: not set; memory: not set |
| mspider-api-service | Global management cluster | Provide interface for Mspider background API interaction and other control behaviors | requests: CPU: not set; memory: not set <br/>limits: CPU: not set; memory: not set |
| Managed mesh | | | |
| istiod-{meshID}-hosted | control plane cluster | policy management for hosted mesh | requests: CPU: 100m; memory: 100m <br/>limits: CPU: not set; memory: not set |
| mspider-mcpc-ckube-remote | Control plane cluster | Invoke remote mesh work clusters to accelerate and aggregate multi-cluster resources | requests: CPU: 100m; memory: 50m<br/>limits: CPU: 500m; memory: 500m |
| mspider-mcpc-mcpc-controller | Control plane cluster | Aggregate mesh multi-cluster related data plane information | requests: CPU: 100m; memory: 0<br/> limits: CPU: 300m; memory: 1.56G |
| {meshID}-hosted-apiserver | Control Plane Cluster | Hosted Control Plane Virtual Cluster API Server | requests: CPU: not set; memory: not set<br/> limits: CPU: not set; memory: not set |
| istiod | working cluster | Mainly used for sidecar lifecycle management of the cluster | requests: CPU: 100; memory: 100<br/> limits: CPU: not set; memory: not set |
| Proprietary mesh | | | |
| istiod | | used for policy creation, delivery, and sidecar lifecycle management | requests: CPU: 100; memory: 100<br/> limits: CPU: not set; memory: not set |
| mspider-mcpc-ckube-remote | working cluster | call remote mesh working cluster | requests: CPU: 100m; memory: 50m<br/> limits: CPU: 500m; memory: 500m |
| mspider-mcpc-mcpc-controller | Working cluster | Collect cluster data surface information | requests: CPU: 100m; memory: 0<br/> limits: CPU: 300m; memory: 1.56G |
| External mesh | | | |
| mspider-mcpc-ckube-remote | working cluster | call remote mesh working cluster | requests: CPU: 100m; memory: 50m<br/> limits: CPU: 500m; memory: 500m |
| mspider-mcpc-mcpc-controller | Working cluster | Collect cluster data surface information | requests: CPU: 100m; memory: 0<br/> limits: CPU: 300m; memory: 1.56G |

The preset resource settings of each control plane component of the service mesh are shown in the table above, and users can find the corresponding work in the [Container Management](../../kpanda/user-guide/workloads/create-deployment.md) module Load, customize CPU and memory resources for the workload.