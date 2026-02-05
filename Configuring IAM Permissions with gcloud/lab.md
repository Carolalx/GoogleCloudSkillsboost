#     Configuring IAM Permissions with gcloud - GSP647

1 - Clique em Start Lab    
2 - Abra o console em janela anonima > insira usuáirio e senha > Clique em Agree and Continue   
3 - Clique para abrir o Cloud Shell >_ (ao lado do ícone do Gemini)   
4 - Copie o código abaixo e cole no terminal   
 
```bash
gcloud compute ssh centos-clean --zone=$(gcloud compute project-info describe --format="value(commonInstanceMetadata.items[google-compute-default-zone])") --quiet
```

```bash
curl -LO https://raw.githubusercontent.com/Carolalx/GoogleCloudSkillsboost/refs/heads/main/Configuring%20IAM%20Permissions%20with%20gcloud/carolalx.sh
sudo chmod +x carolalx.sh
./carolalx.sh
```

5 - Siga os passos solicitados pelo terminal   
6 - Verifique seu progresso
