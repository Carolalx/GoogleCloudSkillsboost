## 🌐 Using the Google Cloud Speech API: Challenge Lab - ARC131 🚀

1 - Clique em `Start Lab`   
2 - Abra o console em janela anonima > insira usuáirio e senha > Clique em `Agree and Continue`   
3 - Clique para abrir o Cloud Shell `>_` (ao lado do ícone do Gemini)   
4 - Execute o código abaixo no terminal

```
export ZONE=$(gcloud compute instances list lab-vm --format 'csv[no-heading](zone)')
gcloud compute ssh lab-vm --project=$DEVSHELL_PROJECT_ID --zone=$ZONE --quiet
```

5 - Clique em `Menu` > `API` > `Credentials` > `+ Create Credential` > `API Key`   
6 - Cole a chave em um bloco de notas    
7 - Execute o comando abaixo no teminal, a primeira solicitação será a chave, recém criada e a sequencia tem nas instruções do lab   

```
curl -LO raw.githubusercontent.com/Carolalx/GoogleCloudSkillsboost/refs/heads/main/Using%20the%20Google%20Cloud%20Speech%20API%3A%20Challenge%20Lab/carolalx.sh
sudo chmod +x carolalx.sh
./carolalx.sh
```

8 - Informe os dados (conforme seu lab) solicitados no terminal   
9 - Verifique seu Progresso! (pode demorar um pouco)

---

🎉 Parabéns! Lab Concluído! 🏆

