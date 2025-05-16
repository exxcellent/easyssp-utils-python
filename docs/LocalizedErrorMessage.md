# LocalizedErrorMessage


## Properties

| Name                  | Type                                                    | Description | Notes      |
|-----------------------|---------------------------------------------------------|-------------|------------|
| **code**              | **int**                                                 |             | [optional] |
| **message**           | **str**                                                 |             | [optional] |
| **details**           | **str**                                                 |             | [optional] |
| **localized_message** | [**ClientLocalizedMessage**](ClientLocalizedMessage.md) |             | [optional] |

## Example

```python
from easyssp_utils.models.localized_error_message import LocalizedErrorMessage
from easyssp_utils.models import LocalizedMessageKey
from easyssp_utils.models.client_localized_message import ClientLocalizedMessage

localized_message_key = LocalizedMessageKey(defaultMessage='Model not found.')
client_localized_message = ClientLocalizedMessage(key=localized_message_key,
                                                  values=['da0e6281-27a8-4708-8679-1abed8df20f4'])
localized_error_message = LocalizedErrorMessage(code=404, message='Model not found',
                                                details='Model with id da0e6281-27a8-4708-8679-1abed8df20f4 not found.',
                                                localizedMessage=client_localized_message)
print(localized_error_message)

# convert the object into a dict
localized_error_message_dict = localized_error_message.to_dict()
# create an instance of LocalizedErrorMessage from a dict
localized_error_message_from_dict = LocalizedErrorMessage.from_dict(localized_error_message_dict)
```
[[Back to README]](../README.md)


