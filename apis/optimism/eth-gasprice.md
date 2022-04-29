---
description: Returns the current price per gas in wei.
---

# eth\_gasPrice - Optimism

{% hint style="info" %}
If you are curious about the difference in gas price between this method and the [eth gas station](https://ethgasstation.info), check out this [GitHub issue](https://github.com/ethereum/go-ethereum/issues/15825).
{% endhint %}

#### Parameters

none

#### Returns

`QUANTITY` - integer of the current gas price in wei.

#### [Example](https://composer.alchemyapi.io/?composer\_state=%7B%22network%22%3A0%2C%22methodName%22%3A%22eth\_gasPrice%22%2C%22paramValues%22%3A%5B%5D%7D)

Request

{% tabs %}
{% tab title="Curl" %}
```bash
curl https://opt-mainnet.g.alchemy.com/v2/your-api-key \
-X POST \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_gasPrice","params":[],"id":0}'
```
{% endtab %}

{% tab title="Postman" %}
```http
URL: https://opt-mainnet.g.alchemy.com/v2/your-api-key
RequestType: POST
Body: 
{
    "jsonrpc":"2.0",
    "method":"eth_gasPrice",
    "params":[],
    "id":0
}
```
{% endtab %}
{% endtabs %}

Result

```javascript
{
    "jsonrpc": "2.0",
    "id": 0,
    "result": "0xe4e1c0"
}
```

{% embed url="https://docs.alchemy.com/alchemy/apis/optimism-api" %}
