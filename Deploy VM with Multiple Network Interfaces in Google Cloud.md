# Deploy VM with Multiple Network Interfaces in Google Cloud

1 - Clique em `Start Lab`   
2 - Copie o código abaixo e cole em um bloco de notas   

```bash
gcloud compute instances create multi-nic-vm --zone=[YOUR REGION] --machine-type=e2-medium --image-family=debian-12 --image-project=debian-cloud --boot-disk-size=20GB --boot-disk-type=pd-balanced --network-interface=network=my-vpc1,subnet=subnet-a,no-address --network-interface=network=my-vpc2,subnet=subnet-b,no-address --tags=multi-nic,internal-vm --labels=env=dev,role=multinic
```

3 - Substitua `[YOUR REGION]`pela região fornecida em seu lab   
4 - Cone no terminal e tecle `ENTER`   
5 - Aguarde a execução e verifique seu progresso.
