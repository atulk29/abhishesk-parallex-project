## APPS-INFRA-MANIFESTS
# Terraform
Commands to be executed for devops pipeline
    
    - cd envs/dev
    - aws sts get-caller-identity
    - find . -type d -name ".terragrunt-cache" -prune -exec rm -rf {} \;
    - terragrunt run-all init --terragrunt-parallelism 1
    - terragrunt run-all validate --terragrunt-parallelism 1
    - terrascan init
    - terrascan scan
    - terragrunt run-all plan --terragrunt-parallelism 1
    - terragrunt run-all apply --terragrunt-parallelism 1 --terragrunt-non-interactive
    - terragrunt run-all destroy  --terragrunt-non-interactive   

aws eks update-kubeconfig --region ap-southeast-1 --name parallaxiq-devqa-workloads



mysql --port 3306 --user=parallaxiq --password="check" -h parallaxiq.cte0eqigeljl.ap-southeast-1.rds.amazonaws.com
 --ssl-ca ~/rds-combined-ca-bundle.pem

 telnet z-1.parallaxiqdevqa.ryp1ym.c4.kafka.ap-southeast-1.amazonaws.com 2181

docker run -it -p 5001:5001 676676413995.dkr.ecr.ap-southeast-1.amazonaws.com/order-management:1
docker run -it -p 5000:5000 676676413995.dkr.ecr.ap-southeast-1.amazonaws.com/wha-orchestrator:1
docker run -it -p 5002:5002 676676413995.dkr.ecr.ap-southeast-1.amazonaws.com/userandclientservice:17