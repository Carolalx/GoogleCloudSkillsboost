## 🌐 Configure Cloud Storage Bucket for Website Hosting using gsutil 🚀

1 - Clique em Start Lab   
2 - Copie o código abaixo e cole em um bloco de notas   
3 - complete a linha com o `BUCKET_NAME` informado em seu lab   
4 - cole no terminal e pressione `ENTER`

```
export BUCKET=
```

---

5 - cole no terminal e pressione `ENTER`
```
gsutil web set -m index.html -e error.html gs://$BUCKET
gsutil uniformbucketlevelaccess set off gs://$BUCKET
gsutil defacl set public-read gs://$BUCKET
gsutil acl set -a public-read gs://$BUCKET/index.html
gsutil acl set -a public-read gs://$BUCKET/error.html
gsutil acl set -a public-read gs://$BUCKET/style.css
gsutil acl set -a public-read gs://$BUCKET/logo.jpg
```
 
6 - Verifique seu Progresso!

---
🎉 Parabéns! Lab Concluído! 🏆


