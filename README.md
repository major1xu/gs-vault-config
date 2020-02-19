# gs-vault-config
https://spring.io/guides/gs/vault-config/

set up env var
export VAULT_TOKEN="00000000-0000-0000-0000-000000000000" 
export VAULT_ADDR="http://127.0.0.1:8200"
vault kv put secret/gs-vault-config example.username=demouser example.password=demopassword
vault kv put secret/gs-vault-config/cloud example.username=clouduser example.password=cloudpassword

start local vault dev server
vault server --dev --dev-root-token-id="00000000-0000-0000-0000-000000000000"
