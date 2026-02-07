# Deploy VM with Multiple Network Interfaces in Google Cloud

1 - Clique em Start Lab   
2 - Abra o console em janela anonima > insira usuáirio e senha > Clique em `Agree and Continue`    
3 - Clique para abrir o Cloud Shell `>_` (ao lado do ícone do Gemini)   
4 - Digite no terminal: (ou copie e cole)  
5 - Substitua `[YOUR REGION]`pela região fornecida em seu lab   

```bash
gcloud compute instances create multi-nic-vm --zone=[YOUR REGION] --machine-type=e2-medium --image-family=debian-12 --image-project=debian-cloud --boot-disk-size=20GB --boot-disk-type=pd-balanced --network-interface=network=my-vpc1,subnet=subnet-a,no-address --network-interface=network=my-vpc2,subnet=subnet-b,no-address --tags=multi-nic,internal-vm --labels=env=dev,role=multinic
```


6 - Aguarde a execução e verifique seu progresso.   


---
🎉 Parabéns! Lab Concluído! 🏆
