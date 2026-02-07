# Enhance Scalability Using Managed Instance Groups 

1 - Clique em Start Lab   
2 - Abra o console em janela anonima > insira usuáirio e senha > Clique em `Agree and Continue`    
3 - Clique para abrir o Cloud Shell `>_` (ao lado do ícone do Gemini)   
4 - Copie o código abaixo, cole em um bloco de notas e substitua `[enter region]` pela região informada em seu lab ⚠️(2 locais)⚠️


```bash
gcloud compute instance-groups managed create dev-instance-group --template=dev-instance-template --size=1 --region=[enter region] && gcloud compute instance-groups managed set-autoscaling dev-instance-group --region=[enter region] --min-num-replicas=1 --max-num-replicas=3 --target-cpu-utilization=0.6 --mode=on
```

5 - Cole em seu terminal e tecle `ENTER`   
6 - Aguarde a execução e verifique seu progresso   

---
🎉 Parabéns! Lab Concluído! 🏆
