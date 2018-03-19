
## Function name : GetMonitorContrast
Group: Monitor Configuration (Vista) - Library: dxva2    
***  


#### Retrieves the minimum, maximum, and current contrast settings for a monitor.
***  


## Declaration:
```foxpro  
BOOL GetMonitorContrast(
  HANDLE  hMonitor,
  LPDWORD  pdwMinimumContrast,
  LPDWORD  pdwCurrentContrast,
  LPDWORD  pdwMaximumContrast
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER GetMonitorContrast IN dxva2;
	INTEGER hMonitor,;
	LONG @pdwMinimumContrast,;
	LONG @pdwCurrentContrast,;
	LONG @pdwMaximumContrast  
```  
***  


## Parameters:
hMonitor
[in]  Handle to a physical monitor. To get the monitor handle, call GetPhysicalMonitorsFromHMONITOR or GetPhysicalMonitorsFromIDirect3DDevice9.

pdwMinimumContrast
[out]  Receives the monitor"s minimum contrast.

pdwCurrentContrast
[out]  Receives the monitor"s current contrast.

pdwMaximumContrast
[out]  Receives the monitor"s maximum contrast.
  
***  


## Return value:
If the function succeeds, the return value is nonzero.  
***  


## Comments:
See also: SetMonitorContrast   
  
***  
