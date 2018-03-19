
## Function name : FindFirstVolumeMountPoint
Group: File System - Library: kernel32    
***  


#### Returns the name of a volume mount point on the specified volume. It is used to begin scanning the volume mount points on a volume.

***  


## Code examples:
[Enumerating Volumes and Volume Mounting Points (NTFS)](../../samples/sample_087.md)  

## Declaration:
```foxpro  
HANDLE FindFirstVolumeMountPoint(
	LPTSTR lpszRootPathName,
	LPTSTR lpszVolumeMountPoint,
	DWORD cchBufferLength
);
  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER FindFirstVolumeMountPoint IN kernel32;
	STRING lpszRootPathName,;
	STRING @lpszVolumeMountPoint,;
	LONG cchBufferLength
  
```  
***  


## Parameters:
lpszRootPathName 
[in] Unique volume name of the volume to scan for volume mount points. A trailing backslash is required. 

lpszVolumeMountPoint 
[out] Pointer to a buffer that receives the name of the first volume mount point found. 

cchBufferLength 
[in] Length of the buffer that receives the volume mount point name, in TCHARs.   
***  


## Return value:
If the function succeeds, the return value is a search handle used in a subsequent call to the FindNextVolumeMountPoint and FindVolumeMountPointClose functions.  
***  


## Comments:
Read article <a href="http://msdn.microsoft.com/library/default.asp?url=/library/en-us/fileio/fs/volume_mount_points.asp">Volume Mount Points</a> on MSDN.  
  
***  
