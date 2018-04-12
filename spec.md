Get from pip using the [Microsoft Azure bundle](https://pypi.python.org/pypi/azure) `pip install azure`. On Windoes installed in direcotry like `C:\Users\{USER_NAME_HERE}\AppData\Roaming\Python\Python27\site-packages\azure\mgmt\iothub`.

**OR**

Stand alone packages via pip install for [`azure-iothub-service-client`](https://pypi.python.org/pypi/azure-iothub-service-client) [Github Repo](https://github.com/Azure/azure-iot-sdk-python/tree/master/service) and [`azure-iothub-device-client`](https://pypi.python.org/pypi/azure-iothub-device-client) [GitHub Repo](https://github.com/Azure/azure-iot-sdk-python/tree/master/device).

## [D2C Messages](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-python-python-file-upload)

- Need to decompose APIs
- Depends on
```python
import iothub_client
from iothub_client import IoTHubClient, IoTHubClientError, IoTHubTransportProvider, IoTHubClientResult, IoTHubError
```
- Uses IoTHubTransportProvider.HTTP protocol to send a file from a client app to the cloud backend in IoT Hub given a connection string.

## [C2D Messages](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-python-python-c2d)

- Need to decompose APIs
- Depends on
```python
import iothub_client
from iothub_client import IoTHubClient, IoTHubClientError, IoTHubTransportProvider, IoTHubClientResult
from iothub_client import IoTHubMessage, IoTHubMessageDispositionResult, IoTHubError
```
- Uses the IoTHubTransportProvider.AMQP or AMQP_WS protocol to send data to a simulatred device in python.

## [Device Twin](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-python-twin-getstarted)

- Need to decompose APIs
- Depends on

  service app
    ```python
    import iothub_service_client
    from iothub_service_client import IoTHubRegistryManager, IoTHubRegistryManagerAuthMethod
    from iothub_service_client import IoTHubDeviceTwin, IoTHubError
    ```
  device app
    ```python
    import iothub_client
    from iothub_client import IoTHubClient, IoTHubClientError, IoTHubTransportProvider, IoTHubClientResult, IoTHubError
    ```
-

## [Method Invocation](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-python-python-direct-methods)

- Need to decompose APIs
- Depends on
```python
import iothub_service_client
from iothub_service_client import IoTHubDeviceMethod, IoTHubError
```
- React to methods invoked by the cloud

## [Choosing a Protocol](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-protocols)

Includes
- MQTT
- MQTT over WebSockets
- AMQP
- AMQP over WebSockets
- HTTPS
