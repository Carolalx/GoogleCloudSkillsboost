## 🌐 Create VPC Peering Connection between VPCs 🚀

1 - Clique em `Start Lab`   
2 - Execute os comandos abaixo, um de cada vez   

```
gcloud auth list

export ZONE=$(gcloud compute project-info describe --format="value(commonInstanceMetadata.items[google-compute-default-zone])")

export PROJECT_ID=$(gcloud config get-value project)

gcloud config set compute/zone "$ZONE"

gcloud compute networks create workspace-vpc --subnet-mode=custom

gcloud compute networks create private-vpc --subnet-mode=custom

gcloud compute networks peerings create workspace-to-private --network=workspace-vpc --peer-network=private-vpc --auto-create-routes

gcloud compute networks peerings create private-to-workspace --network=private-vpc --peer-network=workspace-vpc --auto-create-routes

gcloud compute ssh workspace-vm --project="$PROJECT_ID" --zone="$ZONE"

```

3 - Verifique o seu progresso.

---

🏆 Parabéns!! Laboratório concluído!
