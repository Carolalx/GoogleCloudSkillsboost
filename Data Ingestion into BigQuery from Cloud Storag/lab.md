# 🌐 Data Ingestion into BigQuery from Cloud Storage 🚀

## ☁️ Execute no terminal:
```bash
export BUCKET=  #cole o Bucket informado em seu lab
```
```bash
bq mk work_day && bq load --source_format=CSV --skip_leading_rows=1 work_day.employee gs://$BUCKET/employees.csv employee_id:INTEGER,device_id:STRING,username:STRING,department:STRING,office:STRING
```

</div>

---
## 🎉 **Parabéns! Laboratório Conclupido!** 🏆
