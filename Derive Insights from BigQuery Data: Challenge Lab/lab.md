# 🌐 Derive Insights from BigQuery Data: Challenge Lab - GSP787 🚀

1 - Clique em `Start Lab`      
2 - Clique em `Agree and Continue`   
3 - Clique para abrir o Cloud Shell `>_` (ao lado do ícone do Gemini)   
4 - Execute o código abaixo e cole no terminal:

```bash
curl -LO raw.githubusercontent.com/Carolalx/GoogleCloudSkillsboost/refs/heads/main/Derive%20Insights%20from%20BigQuery%20Data%3A%20Challenge%20Lab/carolalx.sh
sudo chmod +x carolalx.sh
./carolalx.sh
```

5 - Dê as inoformações solicitadas, conforme seu lab,  ao terminal    
6 - Verifique seu progresso, caso conte somente 90 pontos, siga os passos:   
7 - No Menu > `BigQuery`, em `Untitle` cole o código: 

```
SELECT
  DATE(date) AS date
FROM (
  SELECT
    date,
    SUM(cumulative_deceased) AS total_deaths
  FROM
    `bigquery-public-data.covid19_open_data.covid19_open_data`
  WHERE
    country_name = 'Italy'
    AND date >= '2020-01-01'
  GROUP BY
    date
)
WHERE
  total_deaths > 10000
ORDER BY
  date ASC
LIMIT 1;
```

8 - Altere o valor de `total_deaths` para o valor indicado em sua Task 5     
9 - Clique em `Run`  
10 - Verifique seu Progresso   

---
🎉 Parabéns! Lab Concluído! 🏆
