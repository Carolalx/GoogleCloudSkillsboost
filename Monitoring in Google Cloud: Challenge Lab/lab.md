# 🌐 Monitoring in Google Cloud: Challenge Lab || ARC115 🚀

## ☁️ Execute no Cloud Shell:

```bash
curl -LO raw.githubusercontent.com/prateekrajput08/Arcade-Google-Cloud-Labs/refs/heads/main/Monitoring%20in%20Google%20Cloud%3A%20Challenge%20Lab/TechCode.sh
sudo chmod +x TechCode.sh 
./TechCode.sh
```

* Navegue até `Create log-based metric` [aqui](https://console.cloud.google.com/logs/metrics/edit?)

1. Para Log-based metric name: digite `carolalx`

2. Cole o comando a seguir `Build filter` & reescreva com seu PROJECT_ID

```bash
resource.type="gce_instance"
logName="projects/PROJECT_ID/logs/apache-access"
textPayload:"200"
```

3. Cole o comando a seguir em `Regular Expression` :

```bash
execution took (\d+)
```

---

## 🎉 **Parabéns! Laboratório Concluído!** 🏆  
