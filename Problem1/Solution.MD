```
jq -r 'select(.symbol == "TSLA") | .order_id' transaction-log.txt | xargs -I {} curl -X GET "https://example.com/api/{}"
```