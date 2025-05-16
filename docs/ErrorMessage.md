# ErrorMessage


## Properties

| Name        | Type    | Description | Notes      |
|-------------|---------|-------------|------------|
| **code**    | **int** |             | [optional] |
| **message** | **str** |             | [optional] |
| **details** | **str** |             | [optional] |

## Example

```python
from easyssp_utils.models import ErrorMessage

error_message = ErrorMessage(code=404, message='Model not found',
                             details='Model with id da0e6281-27a8-4708-8679-1abed8df20f4 not found.')
print(error_message)

# convert the object into a dict
error_message_dict = error_message.to_dict()
# create an instance of ErrorMessage from a dict
error_message_from_dict = ErrorMessage.from_dict(error_message_dict)
```
[[Back to README]](../README.md)


