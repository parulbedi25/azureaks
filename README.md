# azureaks
1. Create AKS Cluster
2. Connect to AKS Cluster using Cloud Shell
az aks get-credentials --resource-group aksdemo --name aksdemo1  
3. Connect to AKS Cluster using Azure CLI
4. Deploy sample App on AKS
5. Merging two config files:
    export KUBECONFIG=~/.kube/config:~/.kube/aksconfig
    kubectl config view --merge --flatten > ~/.kube/config-merged
    mv ~/.kube/config-merged ~/.kube/config