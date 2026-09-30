# Complete Operation Schema

## 1. Power On Chamber

- **Input:** Power supply
- **Precondition:** Chamber is powered off
- **Processing:** Start the system
- **Postcondition:** System starts successfully

## 2. Perform Sensor Self-Check

- **Input:** Sensor readings
- **Precondition:** Chamber is powered on
- **Processing:** Test all essential sensors
- **Postcondition:** Sensors are marked as working or failed

## 3. Check Environmental-Control Devices

- **Input:** Device status
- **Precondition:** System is powered on
- **Processing:** Test environmental-control devices
- **Postcondition:** Devices are marked ready or not ready

## 4. Register Artifact

- **Input:** Artifact ID and details
- **Precondition:** Artifact is inside the chamber
- **Processing:** Store artifact identification information
- **Postcondition:** Artifact is registered

## 5. Load Environmental Profile

- **Input:** Required temperature and humidity limits
- **Precondition:** Artifact is registered
- **Processing:** Load the artifact's environmental requirements
- **Postcondition:** Environmental profile is loaded

## 6. Check Door Status

- **Input:** Door sensor data
- **Precondition:** Door sensor is working
- **Processing:** Check whether the door is open or closed
- **Postcondition:** Current door status is known

## 7. Monitor Environmental Conditions

- **Input:** Temperature, humidity, light and vibration readings
- **Precondition:** Sensors are working
- **Processing:** Continuously monitor chamber conditions
- **Postcondition:** Current environmental conditions are available

## 8. Compare Temperature with Limits

- **Input:** Current temperature and allowed range
- **Precondition:** Environmental profile is loaded
- **Processing:** Compare actual temperature with required limits
- **Postcondition:** Temperature condition is identified as normal or abnormal

## 9. Compare Humidity with Limits

- **Input:** Current humidity and allowed range
- **Precondition:** Environmental profile is loaded
- **Processing:** Compare actual humidity with required limits
- **Postcondition:** Humidity condition is identified as normal or abnormal

## 10. Correct Temperature

- **Input:** Current temperature and target range
- **Precondition:** Temperature is outside the allowed range
- **Processing:** Activate temperature-control mechanism
- **Postcondition:** Temperature correction command is issued

## 11. Correct Humidity

- **Input:** Current humidity and target range
- **Precondition:** Humidity is outside the allowed range
- **Processing:** Activate humidity-control mechanism
- **Postcondition:** Humidity correction command is issued

## 12. Verify Environmental Recovery

- **Input:** Sensor readings and recovery time
- **Precondition:** Environmental correction has been attempted
- **Processing:** Recheck temperature and humidity
- **Postcondition:** Recovery is confirmed or correction failure is detected

## 13. Detect Vibration

- **Input:** Vibration sensor readings
- **Precondition:** Artifact is inside the chamber
- **Processing:** Check vibration level
- **Postcondition:** Vibration event is detected or not detected

## 14. Verify Vibration Stabilization

- **Input:** Vibration readings and stabilization period
- **Precondition:** Vibration response has started
- **Processing:** Monitor vibration until the required period is completed
- **Postcondition:** Vibration stabilization is confirmed or not confirmed

## 15. Suspend Conservation Activities

- **Input:** Door or vibration event
- **Precondition:** Normal conservation activities are active
- **Processing:** Stop activities that could increase risk
- **Postcondition:** Normal conservation activities are suspended

## 16. Activate Protection Controls

- **Input:** Environmental failure or dangerous condition
- **Precondition:** Normal recovery has failed
- **Processing:** Reduce light exposure and activate additional controls
- **Postcondition:** Protection controls are active

## 17. Generate Operator Alert

- **Input:** Fault or emergency information
- **Precondition:** A serious protection condition exists
- **Processing:** Send an alert to the museum operator
- **Postcondition:** Operator is notified

## 18. Switch to Emergency Power

- **Input:** Main power status
- **Precondition:** Main power is unavailable
- **Processing:** Activate emergency power source
- **Postcondition:** Emergency power is active

## 19. Record Power Failure

- **Input:** Power failure information
- **Precondition:** Main and emergency power are unavailable
- **Processing:** Record the power failure incident
- **Postcondition:** Power failure is recorded

## 20. Perform Safe Shutdown

- **Input:** System status
- **Precondition:** No usable power is available
- **Processing:** Shut down the system safely
- **Postcondition:** System is safely shut down

## 21. Verify Chamber Safety

- **Input:** Environmental readings and protection status
- **Precondition:** Artifact removal has been requested
- **Processing:** Check environmental conditions and active protection responses
- **Postcondition:** Chamber safety is confirmed or rejected

## 22. Authorize Artifact Removal

- **Input:** Safety verification result
- **Precondition:** Chamber is confirmed safe
- **Processing:** Give permission to remove the artifact
- **Postcondition:** Artifact removal is authorized
