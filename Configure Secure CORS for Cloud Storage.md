## 🌐 Configure Secure CORS for Cloud Storage 🚀  

1 - Clique em Start Lab   
2 - Cole o código abaixo no terminal e pressione `ENTER`   

```
echo '[{"origin":["http://example.com"],"method":["GET"],"responseHeader":["Content-Type"],"maxAgeSeconds":3600}]' > cors.json
```

3 - Quando a execução anterior finalizar, cole o código abaixo no terminal e pressione `ENTER`    

```
gcloud storage buckets update gs://$(gcloud config get-value project)-bucket --cors-file=cors.json
```

---
 
🎉 Parabéns! Lab Concluído! 🏆



