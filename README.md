# Kubernetes-cluster-using-Terraform

terraform init
terraform plan
terraform apply

aws eks --region $(terraform output -raw region) update-kubeconfig \
    --name $(terraform output -raw cluster_name)


kubectl cluster-info
kubettl get nodes
