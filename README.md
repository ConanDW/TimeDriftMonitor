# TimeDriftMonitor
Monitor made to make sure servers and workstations are not off. It is made to work with the Datto RMM platform. The script checks what the local time on the endpoint and checks it against a time server. The time server can be set to any time server but the default is "time.windows.com". It also allows you to take up to 10 samples. If the option is selected the script will automatically resync the local endpoint's time. Please see flow chart below.




.SYNOPSIS
    Monitoring - Windows - Time Drift
    
.DESCRIPTION
    This script will monitor time drift on the machine vs a provided "source of truth".
    
.NOTES
    2024-02-15: Modifications by Cameron Day for IPM Computers LLC
    2023-03-22: Exclude empty lines in the output.
    2023-03-18: Add `-Resync` parameter to force a resync if the time drift exceeds threshold.
    2023-03-17: Initial version
    
.LINK
    Original Source: https://kevinholman.com/2017/08/26/monitoring-for-time-drift-in-your-enterprise/
    
.LINK
    Blog post: https://homotechsual.dev/2023/03/17/Monitoring-Time-Drift-PowerShell/

    





![Time Drift Monitor Flow](https://github.com/ConanDW/TimeDriftMonitor/assets/32853335/2bc1a028-db53-44d1-9d1c-a030c5fa04d5)
