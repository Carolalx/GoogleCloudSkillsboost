## 🌐 Configure Cloud CDN for Storage using gcloud 🚀

1 - Clique em Start Lab   
2 - Copie o código abaixo e cole em um bloco de notas   
3 - complete a primeira linha com o `BUCKET_NAME` informado em seu lab   
4 - cole no terminal e pressione `ENTER`

```
BUCKET_NAME=
BACKEND_BUCKET=static-backend-bucket
URL_MAP=cdn-map
PROXY=cdn-http-proxy
FORWARDING_RULE=cdn-http-rule

gcloud compute backend-buckets create $BACKEND_BUCKET --gcs-bucket-name=$BUCKET_NAME --enable-cdn

gcloud compute url-maps create $URL_MAP --default-backend-bucket=$BACKEND_BUCKET
gcloud compute target-http-proxies create $PROXY --url-map=$URL_MAP

gcloud compute forwarding-rules create $FORWARDING_RULE --global --target-http-proxy=$PROXY --ports=80

gcloud compute forwarding-rules describe $FORWARDING_RULE --global --format="value(IPAddress)"
```

---

5 - Substitua `BUCKET_NAME`  pelo código informado em seu lab  
6 - Substitua `IP_ADDRESS` pelo ip gerado no teminal 
7 - cole no terminal e pressione `ENTER
```
gsutil ls gs://BUCKET_NAME/images/
curl -o nature.png http://IP_ADDRESS/images/nature.png
```
 
5 - Verifique seu Progresso!

---
🎉 Parabéns! Lab Concluído! 🏆


