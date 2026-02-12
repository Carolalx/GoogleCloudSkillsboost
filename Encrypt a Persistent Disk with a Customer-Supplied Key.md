## 🌐 Encrypt a Persistent Disk with a Customer-Supplied Key 🚀

1 - Clique em Start Lab   
2 - Copie o código abaixo e cole no terminal

```
export PROJECT_ID=$(gcloud config get-value project) ZONE=$(gcloud compute instances list --limit=1 --format="value(zone)") VM_NAME=$(gcloud compute instances list --limit=1 --format="value(name)") BASE64_KEY=$(head -c 32 /dev/urandom | base64)
gcloud compute disks create csek-encrypted-disk --size=200GB --zone=$ZONE --csek-key-file=<(echo "[{\"uri\": \"https://www.googleapis.com/compute/v1/projects/$PROJECT_ID/zones/$ZONE/disks/csek-encrypted-disk\", \"key\": \"$BASE64_KEY\", \"key-type\": \"raw\"}]")
gcloud compute instances attach-disk $VM_NAME --disk=csek-encrypted-disk --zone=$ZONE --csek-key-file=<(echo "[{\"uri\": \"https://www.googleapis.com/compute/v1/projects/$PROJECT_ID/zones/$ZONE/disks/csek-encrypted-disk\", \"key\": \"$BASE64_KEY\", \"key-type\": \"raw\"}]")
```

🎉 Parabéns! Lab Concluído! 🏆
