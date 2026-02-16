# 🌐 Create Firewall Rule to Enable SSH Access 🚀   

1 - Clique em Start Lab   
2 - Copie o código abaixo e cole no terminal

```
VPC=$(gcloud compute instances describe $(gcloud compute instances list --format="value(name)") --zone=$(gcloud compute instances list --format="value(zone)") --format="value(networkInterfaces[0].network.basename())"); gcloud compute firewall-rules create allow-ssh --network=$VPC --allow=tcp:22 --source-ranges=0.0.0.0/0 --target-tags=http-server
```

---

🎉 Parabéns! Lab Concluído! 🏆

