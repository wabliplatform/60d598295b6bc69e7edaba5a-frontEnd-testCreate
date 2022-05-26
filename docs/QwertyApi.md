# TempApi.QwertyApi

All URIs are relative to *http://83.212.100.226:3002/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createqwerty**](QwertyApi.md#createqwerty) | **POST** /qwerty | Creates the data
[**deleteqwerty**](QwertyApi.md#deleteqwerty) | **DELETE** /qwerty/{qwertyId} | Delete the element
[**getAllqwerty**](QwertyApi.md#getAllqwerty) | **GET** /qwerty/getAll | Get all the data
[**getqwerty**](QwertyApi.md#getqwerty) | **GET** /qwerty/{qwertyId} | Get the element
[**updateqwerty**](QwertyApi.md#updateqwerty) | **PUT** /qwerty/{qwertyId} | Updates the element



## createqwerty

> Qwerty createqwerty(qwerty)

Creates the data

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.QwertyApi();
let qwerty = new TempApi.Qwerty(); // Qwerty | data to be created
apiInstance.createqwerty(qwerty, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **qwerty** | [**Qwerty**](Qwerty.md)| data to be created | 

### Return type

[**Qwerty**](Qwerty.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteqwerty

> deleteqwerty(qwertyId)

Delete the element

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.QwertyApi();
let qwertyId = "qwertyId_example"; // String | the Id parameter
apiInstance.deleteqwerty(qwertyId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **qwertyId** | **String**| the Id parameter | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## getAllqwerty

> [Qwerty] getAllqwerty()

Get all the data

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.QwertyApi();
apiInstance.getAllqwerty((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**[Qwerty]**](Qwerty.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getqwerty

> Qwerty getqwerty(qwertyId)

Get the element

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.QwertyApi();
let qwertyId = "qwertyId_example"; // String | the Id parameter
apiInstance.getqwerty(qwertyId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **qwertyId** | **String**| the Id parameter | 

### Return type

[**Qwerty**](Qwerty.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateqwerty

> Qwerty updateqwerty(qwertyId, opts)

Updates the element

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.QwertyApi();
let qwertyId = "qwertyId_example"; // String | the Id parameter
let opts = {
  'qwerty': new TempApi.Qwerty() // Qwerty | data to be updated
};
apiInstance.updateqwerty(qwertyId, opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **qwertyId** | **String**| the Id parameter | 
 **qwerty** | [**Qwerty**](Qwerty.md)| data to be updated | [optional] 

### Return type

[**Qwerty**](Qwerty.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

