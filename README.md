# kubernetes-setup
Infrastructure architecture and Ansible code for setting up a high availability multi-region Kubernetes cluster with externally exposed applications

# Infrastructure overview
A high availability multi region Kubernetes consists of the following infrastructure components:
* Control Plane and Worker nodes across desired regions
* VNET per region
* VNET peering across regions
* NSG inbound rules
* Internal Load Balancer for HA Control Plane setup 
* External load balancer per region for worker nodes
* Traffic manager to send traffic to the closest region


![image](/diagrams/ha-multi-region-cluster.png)
