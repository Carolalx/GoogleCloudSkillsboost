# 🌐 Configuring IAM Permissions with gCloud - Azure || GSP1119 🚀

1 - Clique em `Start Lab`   
2 - Abra o console em janela anonima > insira usuáirio e senha > Clique em `Agree and Continue`   
3 - Clique para abrir o Cloud Shell `>_` (ao lado do ícone do Gemini)   
4 - Execute o código abaixo no terminal


## ☁️ Execute no Cloud Shell:
```bash
export ZONE=$(gcloud compute instances list --filter="name=centos-clean" --format="value(zone)")
gcloud compute ssh centos-clean --zone=$ZONE --quiet
```

```bash
curl -LO raw.githubusercontent.com/Carolalx/GoogleCloudSkillsboost/refs/heads/main/Configuring%20IAM%20Permissions%20with%20gCloud%20-%20Azure/carolalx.sh
sudo chmod +x carolalx.sh
./carolalx.sh
```

5 - Verifique seu progresso

---

## 🎉 **Parabéns! Laboratório Concluído!** 🏆  
