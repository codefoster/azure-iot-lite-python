Get from pip using the [Microsoft Azure bundle](https://pypi.python.org/pypi/azure) `pip install azure`. On Windoes installed in direcotry like `C:\Users\{USER_NAME_HERE}\AppData\Roaming\Python\Python27\site-packages\azure\mgmt\iothub`.

## [D2C Messages](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-python-python-file-upload)

- Decompose API
- Depends on
```python
import iothub_client
from iothub_client import IoTHubClient, IoTHubClientError, IoTHubTransportProvider, IoTHubClientResult, IoTHubError
```

## [C2D Messages](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-python-python-c2d)

- Need to decompose APIs
- Depends on
```python
import iothub_client
from iothub_client import IoTHubClient, IoTHubClientError, IoTHubTransportProvider, IoTHubClientResult
from iothub_client import IoTHubMessage, IoTHubMessageDispositionResult, IoTHubError
```

## [Device Twin](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-python-twin-getstarted)

- Need to decompose APIs
- Depends on
```python
import iothub_client
from iothub_client import IoTHubClient, IoTHubClientError, IoTHubTransportProvider, IoTHubClientResult, IoTHubError
```

## [Method Invocation](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-python-python-direct-methods)

- Need to decompose APIs
- Depends on
```python
import iothub_service_client
from iothub_service_client import IoTHubDeviceMethod, IoTHubError
```

## [Choosing a Protocol](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-protocols)
