# 🚀 Cloud Run Functions: Qwik Start  - GSP1089 🚀

## APIs Explorer: App Engine - GSP422

1 - Clique em Start Lab   
2 - Abra o console em janela anonima > insira usuáirio e senha > Clique em `Agree and Continue`   
3 - Clique para abrir o Cloud Shell `>_` (ao lado do ícone do Gemini)   
4 - Copie o código abaixo e cole no terminal

---
⚠️VEJA OS PRÓXIMOS ANTES DE DIGITAR `Y`⚠️
---

```
curl -LO raw.githubusercontent.com/Carolalx/GoogleCloudSkillsboost/refs/heads/main/Cloud%20Run%20Functions%3A%20Qwik%20Start/carolalx.sh
sudo chmod +x carolalx.sh 
./carolalx.sh
```

5 - Verifique seu progresso até Task 6. --para completar até a 6 será necessário:   
   - Na barra de pesquisa digite: `Cloud Run Functions`   
   - No menu da esquerda selecione `Services`, escolha o serviço `hello-world-colored`, clique em `Edit & Deploy New Revision`   
   - Em `Variables & Secrets` altere `orange` para **`yellow`**, role a paginá até o fim e clique em `Deploy`<br>
   - Novamente no menu da esquerda selecione `Services`, escolha o serviço `slow-function`, clique em `Edit & Deploy New Revision`     
   - Em `Revision scaling`, `Minimum number of instances ` selecione **`1`** e em `Maximum number of instances` selecione **`4`**  role a paginá até o fim e clique em `Deploy`<br>     
6 - Retorne ao terminal e digite `Y` e `ENTER`   
7 - Após completar a execução...   
   - No menu da esquerda selecione `Services`, escolha o serviço `slow-concurrent-function`, clique em `Edit & Deploy New Revision`  
   - Em `Resources` > `CPU` selecione **`1`**,
   - Em `Requests` > `Maximum concurrent requests per instance` digite **`100`**,   
   - Em `Revision scaling` > `Maximum number of instances` digite **`4`**,
   -   role a paginá até o fim e clique em `Deploy`<br>

8 - Verifique seu progresso.   
   

🎉 Parabéns! Lab Concluído! 🏆
