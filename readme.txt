by :reza ganji

#start vault server in dev mode

vault server --dev --dev-root-token-id="00000000-0000-0000-0000-000000000000"


#in new window

#1
export VAULT_ADDR=http://127.0.0.1:8200

#2
vault kv put secret/tosancloudclient username=tttttttt password=yyyyyyyy


#test
curl -X "GET" "http://localhost:8888/tosancloudclient/default" -H "X-Config-Token: 00000000-0000-0000-0000-000000000000"