# kubeflowbasics
# Shows the last employed pod
kubectl get pods -n kubeflow --sort-by=.metadata.creationTimestamp | tail -n 1
# Shows the logs
kubectl logs -n kubeflow my-pipeline-hnl62-506235080 

# Integration of local containers with your kubernetess:

docker build -t download_and_extract_frames_with_open:latest .
kind load docker-image download_and_extract_frames_with_open:latest


