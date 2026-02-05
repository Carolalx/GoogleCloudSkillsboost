# Google Kubernetes Engine Security: Binary Authorization - GSP479   

***⚠️  Este LAB é um pouco mais complexo, leia tudo antes de exectuar!***   

1 - Clique em Start Lab   
2 - Abra o console em janela anonima > insira usuáirio e senha > Clique em Agree and Continue   
3 - Clique para abrir o Cloud Shell `>_` (ao lado do ícone do Gemini)   
4 - Digite no terminal: (ou copie e cole)   
```bash
gcloud config set project VALUE
```

5 - Copie do LAB as informações de Region and ZONE:  --⚠️varia de LAB para LAB--   

```
gcloud config set compute/region europe-west1
gcloud config set compute/zone europe-west1-c
```

6 - Depois copie o código:   
```
gcloud config set project PROJECT_ID
```
**⚠️ SUBSTITUA `PROJECT_ID` PELO DISPONIBILZADO EM SEU LAB   

7 - Copie o código a seguir e cole no teminal:   

```bash
curl -LO https://raw.githubusercontent.com/Carolalx/GoogleCloudSkillsboost/refs/heads/main/Google%20Kubernetes%20Engine%20Security%3A%20Binary%20Authorization/carolalx.sh
sudo chmod +x carolalx.sh
./carolalx.sh

```

8 - Digite `y` e aguarde   
9 - ⚠️ Aparecerá uma URL, clique nela **ANTES DE DIGITAR `Y` PELA SEGUNDA VEZ**   
10 - Vá em `EDIT POLICY`, desça até `GKE cluster-specific rules `, clique no trẽs potinhos > Edit > Require (...) > by ID   
11 - cole o ID acima da URL do teminal, cole no espaço do ID > ADD > Submit > Save Policy   
12 - Volte ao terminal, digite `Y` e aguarde.   
13 - Verifique seu progresso.


