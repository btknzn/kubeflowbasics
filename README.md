# kubeflowbasics
# Shows the last employed pod
kubectl get pods -n kubeflow --sort-by=.metadata.creationTimestamp | tail -n 1
# Shows the logs
kubectl logs -n kubeflow my-pipeline-hnl62-506235080 
