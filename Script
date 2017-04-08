# A simple Windows 10 script that disables unnecessary and vulnerable services
@echo off
echo Checking if you have Administrative permissions
net sessions
if %errorlevel%==0 (
	echo You have Administrator permissions, running script
) else (
	echo You do not have Administrator permissions, please run again as Administrator...
	pause
	exit
)

echo This script will disable several Windows services. It's your responsibility to understand the 
echo consequences of disabling these services. If you agree, press any key to continue.

pause

echo Turning off Remote Registry
sc config "RemoteRegistry" start= disabled
timeout 2

echo Turning off Offline Files
sc config "CscService" start= disabled
timeout 2

echo Turning off Fax
sc config "Fax" start= disabled
timeout 2

echo Turning off Remote Access Auto Connection Manager
sc config "RasAuto" start= disabled
timeout 2

echo Turning off Remote Access Connection Manager
sc config "RasMan" start= disabled
timeout 2

echo Turning off Remote Desktop Configuration
sc config "SessionEnv" start= disabled
timeout 2

echo Turning off Remote Desktop Services
sc config "TermService" start= disabled
timeout 2

echo Turning off Remote Desktop Services UserMode Port Redirector
sc config "UmRdpService" start= disabled
timeout 2

echo Turning off Routing and Remote Access
sc config "RemoteAccess" start= disabled
timeout 2

echo Turning off Retail Demo Service
sc config "RetailDemo" start= disabled
timeout 2

echo Turning off Secondary Logon
sc config "seclogon" start= disabled
timeout 2

echo Turning off Smart Card
sc config "SCardSvr" start= disabled
timeout 2

echo Turning off Smart Card Device Enumeration Service
sc config "ScDeviceEnum" start= disabled
timeout 2

echo Turning off Smart Card Removal Policy
sc config "SCPolicySvc" start= disabled
timeout 2

echo Turning off Telephony
sc config "TapiSrv" start= disabled
timeout 2

echo Turning off Windows Search
sc config "WSearch" start= disabled
timeout 2

echo Turning off Xbox Live Auth Manager
sc config "XblAuthManager" start= disabled
timeout 2

echo Turning off Xbox Live Game Save
sc config "XblGameSave" start= disabled
timeout 2

echo Turning off Xbox Live Networking Service
sc config "XboxNetApiSvc" start= disabled
timeout 2

echo Turning off Certificate Propagation
sc config "CertPropSvc" start= disabled
timeout 2

echo Turning off IP Helper
sc config "iphlpsvc" start= disabled
timeout 2

echo Turning off Phone Service
sc config "PhoneSvc" start= disabled
timeout 2

echo Turning off TCP/IP NetBIOS Helper
sc config "lmhosts" start= disabled

echo All done! Press any key to exit.
pause
exit
