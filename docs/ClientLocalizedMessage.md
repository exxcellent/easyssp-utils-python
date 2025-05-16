# ClientLocalizedMessage


## Properties

| Name       | Type                                              | Description | Notes      |
|------------|---------------------------------------------------|-------------|------------|
| **key**    | [**LocalizedMessageKey**](LocalizedMessageKey.md) |             | [optional] |
| **values** | **List[object]**                                  |             | [optional] |

## Example

```python
from easyssp_utils.models.client_localized_message import ClientLocalizedMessage, LocalizedMessageKey

localized_message_key = LocalizedMessageKey(defaultMessage='Model not found.')
client_localized_message = ClientLocalizedMessage(key=localized_message_key,
                                                  values=['da0e6281-27a8-4708-8679-1abed8df20f4'])
print(client_localized_message)

# convert the object into a dict
client_localized_message_dict = client_localized_message.to_dict()
# create an instance of ClientLocalizedMessage from a dict
client_localized_message_from_dict = ClientLocalizedMessage.from_dict(client_localized_message_dict)
```
[[Back to README]](../README.md)


