# 🌐 Streaming Analytics into BigQuery: Challenge Lab || ARC106 🚀

1 - Clique em `Start Lab`   
2 - Abra o console em janela anonima > insira usuáirio e senha > Clique em `Agree and Continue`   
3 - Clique para abrir o Cloud Shell `>_` (ao lado do ícone do Gemini)   
4 - Execute o código abaixo no terminal

## ☁️ Execute no Cloud Shell:

```
export BUCKET_NAME=

export DATASET_NAME=

export TABLE_NAME=

export TOPIC_NAME=



gsutil mb gs://$BUCKET_NAME

bq mk $DATASET_NAME

bq mk --table \
$DEVSHEL_PROJECT_ID:$DATASET_NAME.$TABLE_NAME \
data:string

gcloud pubsub topics create $TOPIC_NAME

gcloud pubsub subscriptions create $TOPIC_NAME-sub --topic=$TOPIC_NAME
```

```bash
curl -LO raw.githubusercontent.com/Carolalx/GoogleCloudSkillsboost/refs/heads/main/Streaming%20Analytics%20into%20BigQuery%3A%20Challenge%20Lab/carolalx.sh
sudo chmod +x carolalx.sh
./carolalx.sh
```

5 - Verifique seu progresso

---

## 🎉 **Parabéns! Laboratório Concluído!** 🏆  
