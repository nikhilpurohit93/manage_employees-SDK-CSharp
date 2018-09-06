# IO.Swagger.Api.ContractorsApi

All URIs are relative to *https://mg-eval-test.apigee.net/demo/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ContractorsEmployeeIDDelete**](ContractorsApi.md#contractorsemployeeiddelete) | **DELETE** /contractors/{employeeID} | Deletes an Employee record
[**ContractorsEmployeeIDGet**](ContractorsApi.md#contractorsemployeeidget) | **GET** /contractors/{employeeID} | Retrieves an Employee record
[**ContractorsGet**](ContractorsApi.md#contractorsget) | **GET** /contractors | Retrieves all Employee records
[**ContractorsPost**](ContractorsApi.md#contractorspost) | **POST** /contractors | Creates an Employees


<a name="contractorsemployeeiddelete"></a>
# **ContractorsEmployeeIDDelete**
> void ContractorsEmployeeIDDelete (int? employeeID)

Deletes an Employee record

Deletes the profile of an employee.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ContractorsEmployeeIDDeleteExample
    {
        public void main()
        {
            // Configure API key authorization: Bearer
            Configuration.Default.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // Configuration.Default.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new ContractorsApi();
            var employeeID = 56;  // int? | The unique ID of employee.

            try
            {
                // Deletes an Employee record
                apiInstance.ContractorsEmployeeIDDelete(employeeID);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ContractorsApi.ContractorsEmployeeIDDelete: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **employeeID** | **int?**| The unique ID of employee. | 

### Return type

void (empty response body)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="contractorsemployeeidget"></a>
# **ContractorsEmployeeIDGet**
> Employee ContractorsEmployeeIDGet (int? employeeID)

Retrieves an Employee record

Retrieves the profile of an employee.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ContractorsEmployeeIDGetExample
    {
        public void main()
        {
            // Configure API key authorization: Bearer
            Configuration.Default.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // Configuration.Default.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new ContractorsApi();
            var employeeID = 56;  // int? | The unique ID of employee.

            try
            {
                // Retrieves an Employee record
                Employee result = apiInstance.ContractorsEmployeeIDGet(employeeID);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ContractorsApi.ContractorsEmployeeIDGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **employeeID** | **int?**| The unique ID of employee. | 

### Return type

[**Employee**](Employee.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="contractorsget"></a>
# **ContractorsGet**
> void ContractorsGet ()

Retrieves all Employee records

Retrieves the profile of all employees.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ContractorsGetExample
    {
        public void main()
        {
            // Configure API key authorization: Bearer
            Configuration.Default.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // Configuration.Default.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new ContractorsApi();

            try
            {
                // Retrieves all Employee records
                apiInstance.ContractorsGet();
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ContractorsApi.ContractorsGet: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="contractorspost"></a>
# **ContractorsPost**
> void ContractorsPost (Employee employee = null)

Creates an Employees

Registers a new employee for the client.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ContractorsPostExample
    {
        public void main()
        {
            // Configure API key authorization: Bearer
            Configuration.Default.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // Configuration.Default.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new ContractorsApi();
            var employee = new Employee(); // Employee | The Employee (optional) 

            try
            {
                // Creates an Employees
                apiInstance.ContractorsPost(employee);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ContractorsApi.ContractorsPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **employee** | [**Employee**](Employee.md)| The Employee | [optional] 

### Return type

void (empty response body)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

