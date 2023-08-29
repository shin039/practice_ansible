### 実行コマンド その１

```
# Ansible 実行例
ansible-playbook -i inventory/dev playbook/develop/test.yml --ask-vault-pass

# 停止
docker compose down -v
# rmiも消したいとき
docker compose down -v --rmi all
docker compose down -v --rmi local
```
