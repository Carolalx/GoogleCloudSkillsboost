# 🌐 Cloud Speech API 3 Ways: Challenge Lab || ARC132 🚀

1 - Clique em `Start Lab`      
2 - Abra o console em janela anonima > insira usuáirio e senha > Clique em `Agree and Continue`     
3 - Clique para abrir o Cloud Shell `>_` (ao lado do ícone do Gemini)   
4 - Execute o código abaixo no terminal

```bash
export ZONE=$(gcloud compute instances list lab-vm --format 'csv[no-heading](zone)')
gcloud compute ssh lab-vm --project=$DEVSHELL_PROJECT_ID --zone=$ZONE --quiet
```

```bash
curl -LO 
sudo chmod +x TechCode.sh 
./TechCode.sh
```


---

## **🎉 Parabéns! Lab Concluído! 🏆**
