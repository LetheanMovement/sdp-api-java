# VpnApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**startLetheand**](VpnApi.md#startLetheand) | **GET** /letheand/start | 


<a name="startLetheand"></a>
# **startLetheand**
> startLetheand(dataDir, version)



### Example
```java
// Import classes:
import org.lethean.sdp.ApiClient;
import org.lethean.sdp.ApiException;
import org.lethean.sdp.Configuration;
import org.lethean.sdp.models.*;
import org.lethean.api.VpnApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    VpnApi apiInstance = new VpnApi(defaultClient);
    String dataDir = "dataDir_example"; // String | Returns the binary version
    Boolean version = true; // Boolean | Returns the binary version
    try {
      apiInstance.startLetheand(dataDir, version);
    } catch (ApiException e) {
      System.err.println("Exception when calling VpnApi#startLetheand");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dataDir** | **String**| Returns the binary version |
 **version** | **Boolean**| Returns the binary version | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

