# ACM
This repo contains useful files when working with Advanced cluster managment


### Policy description

This policy enforces OpenShift GitOps plus the correct cluster configuration across one of multiple clusters. The relationship between the cluster and the cluster configuration to select will be specified by labeling clusters in RHACM. Cluster labels can be applied whenever you create or import a cluster by setting a value for *appOfAppsPath*.

This policy will do the following

 1. Create *plattform-gitops* namespace and add required RBAC
 2. Deploy *OpenShift-GitOps* operator
 3. Create an ArgoCD instance
 4. Deploy Cluster-configuration based on *appOfAppsPath* value



