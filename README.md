Auto-deployment in minikube with Argocd

Installing ArgoCD on minikube: ( Minikube is already installed in my laotop and start using docker driver)

Step 1: minikube start 

Step 2: kubectl create ns argocd (ArgoCD requires a namespace with its name. Therefore, we will create a namespace for argocd)

Step 3: Apply ArgoCD manifest installation file from ArgoCD github repository
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/v2.9.0/manifests/ha/install.yaml