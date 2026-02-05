# Enhance Scalability Using Managed Instance Groups 

1 - Clique em `Start Lab`   
2 - copie o código abaixo, cole em um bloco de notas e substitua `[enter region]` pela região informada em seu lab (2 locais)

```bash
gcloud compute instance-groups managed create dev-instance-group --template=dev-instance-template --size=1 --region=[enter region] && gcloud compute instance-groups managed set-autoscaling dev-instance-group --region=[enter region] --min-num-replicas=1 --max-num-replicas=3 --target-cpu-utilization=0.6 --mode=on
```

3 - cole em seu terminal e tecle `ENTER`   
4 - Aguarde a execução e verifique seu progresso   
