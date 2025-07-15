# env-var-configmap-k8
This project explores the power of K8
This was a nodejs application where I created a persistent volume  and use persistentVolumeClaim to claim the volume in the pod. I use an environment variables and use configMap in this project just to mimic a complex application where different teams work on deployment.yaml, service.yaml and so on differently.

So with this in mind I wrote each yaml file differently as follows:
1. deployment.yaml for the pods creation, when kube control apply this file, it create the deployment
2. service.yaml for the service creation
3. host-pv.yaml for the host persistentVolume
4. host-pvc.yaml was also created to cliam the persistent Volume and lastly,
5. the environment.yaml file was created for ease of configuration. We wouldn't have needed this in this project but just to mimic working in team on a more complex project.
