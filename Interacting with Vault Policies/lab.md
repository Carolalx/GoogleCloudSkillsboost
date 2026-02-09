# 🌐 Interacting with Vault Policies || GSP1004 🚀 [![Open Lab](https://img.shields.io/badge/Open-Lab-blue?style=flat)](https://www.skills.google/games/6959/labs/43212)


<div style="padding: 15px; margin: 10px 0;">

## ☁️ Rode no Cloud Shell:

```bash
curl -LO https://raw.githubusercontent.com/Carolalx/GoogleCloudSkillsboost/refs/heads/main/Interacting%20with%20Vault%20Policies/carolax1.sh
sudo chmod +x carolax1.sh
./carolax1.sh
```

## ⚠️Abra um segundo teminal Cloud Shell e rode:

```bash
run() {
  echo -e "\n\033[1;36m▶ $*\033[0m"
  "$@"
  echo -e "\n\033[1;33mPress ENTER to continue...\033[0m"
  read
}

export VAULT_ADDR='http://127.0.0.1:8200'
run vault status
printf "\033[1;32mEnter Vault Token: \033[0m"
read -s ROOT_TOKEN
echo
run vault login token="$ROOT_TOKEN"
run vault secrets list
run vault auth enable userpass
run vault write auth/userpass/users/example-user password='password!'
run vault login -method=userpass username=example-user password='password!'
run vault secrets list
echo -e "\n\033[1;32mAll commands completed. Shell will stay open.\033[0m"
exec bash

```
## 👉Create Policy `demo-policy`
⚠️ Preste atenção nesta etapa!! Aqui você do Token gerado nesta mesma execução!   
```bash
path "sys/mounts" {
    capabilities = ["read"]
}
```
## 👉Gera o Token's Policies `demo-policy`

```bash
run() {
  echo -e "\n\033[1;36m▶ $*\033[0m"
  "$@"
  echo -e "\n\033[1;33mPress ENTER to continue...\033[0m"
  read
}

run vault secrets list
run vault login -method=userpass username=example-user password='password!'
run vault secrets list
printf "\033[1;32mEnter Vault Token: \033[0m"
read -s YOUR_TOKEN
echo
run vault token capabilities "$YOUR_TOKEN" sys/mounts
run vault token capabilities "$YOUR_TOKEN" sys/policies/acl
run vault policy list

```
## 👉Edit Policy `demo-policy`
```bash
path "sys/policies/acl" {
    capabilities = ["read", "list"]
}
```

```bash
run() {
  echo -e "\n\033[1;36m▶ $*\033[0m"
  "$@"
  echo -e "\n\033[1;33mPress ENTER to continue...\033[0m"
  read
}

run vault policy list
vault policy list > policies.txt
echo "policies.txt created"
run vault token capabilities "$YOUR_TOKEN" sys/policies/acl
vault token capabilities "$YOUR_TOKEN" sys/policies/acl > token_capabilities.txt
echo "token_capabilities.txt created"
export PROJECT_ID=$(gcloud config get-value project)
run gsutil cp policies.txt token_capabilities.txt "gs://$PROJECT_ID"
```


```bash
curl -LO https://raw.githubusercontent.com/Carolalx/GoogleCloudSkillsboost/refs/heads/main/Interacting%20with%20Vault%20Policies/caroalx2.sh
sudo chmod +x caroalx2.sh 
./caroalx2.sh
```

## 👉Crie as politicas de admin conforme Task 7.

```bash
curl -LO https://raw.githubusercontent.com/Carolalx/GoogleCloudSkillsboost/refs/heads/main/Interacting%20with%20Vault%20Policies/carolalx3.sh
sudo chmod +x carolalx3.sh 
./carolalx3.sh
```

</div>

---

## 🎉 **Congratulations! Lab Completed Successfully!** 🏆  
    <em>Last updated: December 2025</em>
  </p>
</div>
