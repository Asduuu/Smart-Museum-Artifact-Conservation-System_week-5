# Operation Schema

## Smart Museum Artifact Conservation System

| ID | Precondition | Events / Input | Postconditions |
|---|---|---|---|
| OP-01 | Chamber is powered off | Power-on command / power supply | Chamber system is started |
| OP-02 | Chamber is powered on | Sensor readings and self-check request | Essential sensors are verified as working or failed |
| OP-03 | Chamber is powered on | Environmental-control device status | Control devices are verified as ready or not ready |
| OP-04 | Artifact is placed inside the chamber | Artifact ID and identification information | Artifact information is recorded |
| OP-05 | Artifact is registered | Required temperature and humidity limits | Artifact environmental profile is loaded |
| OP-06 | Door sensor is working | Door sensor reading | Current door status is determined |
| OP-07 | Required sensors are working | Temperature, humidity, light, and vibration readings | Current environmental conditions are available |
| OP-08 | Environmental profile is loaded | Current temperature and permitted temperature range | Temperature is identified as normal or abnormal |
| OP-09 | Environmental profile is loaded | Current humidity and permitted humidity range | Humidity is identified as normal or abnormal |
| OP-10 | Temperature is outside the permitted range | Current temperature and target range | Temperature-control correction is activated |
| OP-11 | Humidity is outside the permitted range | Current humidity and target range | Humidity-control correction is activated |
| OP-12 | Correction has been attempted | New temperature and humidity sensor readings | Environmental recovery is confirmed or failure is detected |
| OP-13 | Artifact is inside the chamber | Vibration sensor reading | Vibration event is detected or not detected |
| OP-14 | Vibration response has started | Continuous vibration readings and stabilization period | Vibration stabilization is confirmed or rejected |
| OP-15 | Conservation activities are active | Door-open or significant-vibration event | Risky conservation activities are suspended |
| OP-16 | Environmental recovery has failed or serious condition exists | Protection condition and sensor readings | Additional protection controls are activated |
| OP-17 | Protection condition or serious fault exists | Fault/event information | Museum operator receives an alert |
| OP-18 | Main power is unavailable | Main power failure and emergency power availability | System switches to emergency power |
| OP-19 | Main and emergency power are unavailable | Power failure information | Power failure incident is recorded |
| OP-20 | No usable power is available | Shutdown request / power failure | Chamber system is safely shut down |
| OP-21 | Artifact removal is requested | Environmental readings and protection status | Chamber safety is confirmed or rejected |
| OP-22 | Chamber is confirmed safe and no protection response is active | Artifact removal request | Artifact removal is authorized |
- **Processing:** Give permission to remove the artifact
- **Postcondition:** Artifact removal is authorized
