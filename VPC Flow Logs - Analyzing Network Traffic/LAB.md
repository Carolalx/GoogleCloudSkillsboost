# VPC Flow Logs - Analyzing Network Traffic - GSP212

1 - Clique em Start Lab   
2 - Abra o console em janela anonima > insira usuáirio e senha > Clique em `Agree and Continue`    
3 - Clique para abrir o Cloud Shell `>_` (ao lado do ícone do Gemini)   
4 - Copie o código abaixo e cole no terminal   

```
curl -LO https://raw.githubusercontent.com/Carolalx/GoogleCloudSkillsboost/refs/heads/main/VPC%20Flow%20Logs%20-%20Analyzing%20Network%20Traffic/carolalx.sh
sudo chmod +x carolalx.sh 
./carolalx.sh
```

5 - Antes de digitar `Y` acesse o **1º** link apresentado no Shell   
6 - em **Firewall Rules detais** clique em `Edit`   
7 - em **Logs** selecione `On`   
8 - Clique em `Save`   
9 - Retorne ao Shell e clique no **2º** link apresentado no Shell   
10 - No canto superior direito, clique em `Run Query`   
11 - Clique em `Actions` > `Create sink`   
12 - Nomeie como: `vpc-flows` > clique em `Next`    
13 - em **Select sink service** selecione `BigQuery dataset`   
14 - em **BigQuery dataser** selecione `bq_vpcflows` > `Next` > `Next` > `Create sink`   
15 - Aguarde a mensagem de confirmação   
16 - Retorne ao Shell, Digite `Y` e pressione `ENTER`   


**Sink Name: vpc-flows**
```
export ZONE=$(gcloud compute instances list --filter="name=centos-clean" --format="value(zone)")
gcloud compute ssh centos-clean --zone=$ZONE --quiet
```
