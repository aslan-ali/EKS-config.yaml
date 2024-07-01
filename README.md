If you want to deploy load balancers to a subnet, the subnet must have the following tag:
Private subnets
Key	Value
kubernetes.io/role/internal-elb	1
Public subnets
Key	Value
kubernetes.io/role/elb	1

eks create cluster -f eks-config.yaml
