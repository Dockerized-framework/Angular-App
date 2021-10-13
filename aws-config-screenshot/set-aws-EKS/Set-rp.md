# https://www.youtube.com/watch?v=S8U7A-eGdOs

# https://aws.amazon.com/premiumsupport/knowledge-center/eks-alb-ingress-controller-setup/ 

# https://docs.aws.amazon.com/eks/latest/userguide/enable-iam-roles-for-service-accounts.html

Manifest:
https://github.com/RobinNagpal/kubernetes-tutorials/tree/master/06_tools/007_alb_ingress/01_eks/k8s 

setup EKS on AWS

account ID 627348467762
 
 https://eksctl.io/usage/minimum-iam-policies/
 
 eks-user
 accessID: XXXXX
 secrets: wa0JXXXXXXXXXXXXXX
 
#get kubeconfig 
aws eks --region us-east-2 update-kubeconfig --name labbal-k8s
 
 #node group policy: from EC2
 1.AmazonEKS_CNI_Policy
 2. AmazonEKSWorkerNodePolicy
 3. AmazonEC2ContainerRegistryReadOnly
 

 
#get kubeconfig 
aws eks --region us-east-2 update-kubeconfig --name labbal-k8s

#install ALB ingress using helm without service account
https://artifacthub.io/packages/helm/aws/aws-load-balancer-controller
 