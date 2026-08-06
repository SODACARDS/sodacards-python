# ProblemDetails

An RFC 9457 problem document. Every error response uses this shape. Switch on `code` (stable, machine-readable), never on `title` or `detail` (human copy, may change). `status` mirrors the HTTP status.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** | A URI identifying the error type, e.g. https://developer.sodacards.com/errors/insufficient_balance. | 
**title** | **str** | A short, human-readable summary of the error. | 
**status** | **int** | The HTTP status code, repeated for convenience. | 
**code** | **str** | A stable, machine-readable error code, e.g. insufficient_balance. Switch on this. | 
**detail** | **str** | A human-readable explanation specific to this occurrence. | [optional] 
**request_id** | **str** | The request identifier, to quote when contacting support. | [optional] 

## Example

```python
from sodacards.models.problem_details import ProblemDetails

# TODO update the JSON string below
json = "{}"
# create an instance of ProblemDetails from a JSON string
problem_details_instance = ProblemDetails.from_json(json)
# print the JSON string representation of the object
print(ProblemDetails.to_json())

# convert the object into a dict
problem_details_dict = problem_details_instance.to_dict()
# create an instance of ProblemDetails from a dict
problem_details_from_dict = ProblemDetails.from_dict(problem_details_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


