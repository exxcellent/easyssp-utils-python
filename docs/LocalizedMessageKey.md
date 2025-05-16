# LocalizedMessageKey


## Properties

| Name                | Type    | Description | Notes      |
|---------------------|---------|-------------|------------|
| **default_message** | **str** |             | [optional] |

## Example

```python
from easyssp_utils.models import LocalizedMessageKey

localized_message_key = LocalizedMessageKey(defaultMessage='Model not found.')
print(localized_message_key)

# convert the object into a dict
localized_message_key_dict = localized_message_key.to_dict()
# create an instance of LocalizedMessageKey from a dict
localized_message_key_from_dict = LocalizedMessageKey.from_dict(localized_message_key_dict)
```
[[Back to README]](../README.md)


