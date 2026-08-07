# Problem

An RFC 9457 problem+json error. Switch on `code`, the stable machine-readable reason; the HTTP status frames the broad category.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** | A stable URI identifying the error kind; it resolves to the docs section for that code. | 
**title** | **str** | A short, human-readable summary of the error kind. | 
**status** | **int** | The HTTP status code, repeated in the body for convenience. | 
**code** | **str** | The machine-readable reason (e.g. \&quot;insufficient_balance\&quot;): switch on this, never on the human text. | 
**detail** | **str** | A human-readable explanation of this specific occurrence. May be absent. | [optional] 
**request_id** | **str** | Identifies this request in support conversations. May be absent. | [optional] 

## Example

```python
from sodacards.models.problem import Problem

# TODO update the JSON string below
json = "{}"
# create an instance of Problem from a JSON string
problem_instance = Problem.from_json(json)
# print the JSON string representation of the object
print(Problem.to_json())

# convert the object into a dict
problem_dict = problem_instance.to_dict()
# create an instance of Problem from a dict
problem_from_dict = Problem.from_dict(problem_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


