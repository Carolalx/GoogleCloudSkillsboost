🌐 Assign External IP to VM Instance using gcloud 🚀   

1 - Clique em Start Lab   
2 - Copie o código abaixo e cole no terminal

```
export VM_NAME=$(gcloud compute instances list --format='value(name)' --limit=1) && export ZONE=$(gcloud compute instances list --format='value(zone)' --limit=1) && export REGION=${ZONE%-*}
gcloud compute addresses create lab-static-ip --region=$REGION
export IP_ADDRESS=$(gcloud compute addresses describe lab-static-ip --region=$REGION --format='get(address)') && gcloud compute instances add-access-config $VM_NAME --zone=$ZONE --address=$IP_ADDRESS
```

🎉 Parabéns! Lab Concluído! 🏆

