# Create token

curl -s -k -X POST https://10.43.0.55:4444/api/com.ibm.zaci.system/api-tokens/  \
-H 'zaci-api: com.ibm.zaci.system/1.0'  \
-H 'accept: application/vnd.ibm.zaci.payload+json'  \
-H 'Content-type: application/vnd.ibm.zaci.payload+json;version=1.0'  \
-d '{"kind": "request", "parameters": { "user": "root" , "password": "password" } }'

# Appliance API

curl -k -X GET https://10.43.0.55:4444/api/com.ibm.zaci.system/appliance \
    -H "Authorization: Bearer $token" \
    -H "zACI-API: com.ibm.zaci.system/1.0" \
    -H "Accept: application/vnd.ibm.zaci.payload+json;version=1.0"
