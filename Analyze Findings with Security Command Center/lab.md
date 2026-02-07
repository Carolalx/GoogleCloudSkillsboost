# Analyze Findings with Security Command Center - GSP1164

1 - Clique em Start Lab   
2 - Abra o console em janela anonima > insira usuáirio e senha > Clique em `Agree and Continue`   
3 - Clique para abrir o Cloud Shell `>_` (ao lado do ícone do Gemini)   
4 - Copie o código abaixo e cole no terminal   

```
curl -LO https://raw.githubusercontent.com/Carolalx/GoogleCloudSkillsboost/refs/heads/main/Analyze%20Findings%20with%20Security%20Command%20Center/carolalx.sh
sudo chmod +x carolalx.sh 
./carolalx.sh

```
⚠️ ⚠️ 
5 - Antes de digitar `Y`, clique no link apresentado no terminal   
   - Em **Continuous Export Name** digite: `export-findings-pubsub-topic`;       
   - Em **Export To**, clique em **Select**, selecione o usuário apresentado;   
   - Em **Select a cloud Pub/Sub Topic**, selecione o usuário novamente;
   - Pressione `Save`;
   - Após ver **Active ✅** em status, retorne ao terminal, digite `Y` e pressione `Enter`.

6 - Quanto no terminal aparecer `No findings yet. Wainting for 100 seconds`, pressione `CTRL`+ `C`   
    chame novamente: `./carolalx.sh`   

7 - Desta vez, digite `Y` e tecle ENTER sem acessar o link 
8 - Quando finalizar a execução no terminal, clique no link apresentado   
9 - Siga os passos da Task 2. do título `Create a table in Big Query`  


---
🎉 Parabéns! Lab Concluído! 🏆

   
