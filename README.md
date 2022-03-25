# windows10-windows-update-policies

```reg
Windows Registry Editor Version 5.00

[HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\WindowsUpdate]
"ProductVersion"="Windows 10"
"TargetReleaseVersion"=dword:00000001
"TargetReleaseVersionInfo"="21H2"

```

![image](https://user-images.githubusercontent.com/1501327/160027519-c956f2fa-bf4d-440b-ac54-7b1e32808bea.png)

```bat
reg add HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\WindowsUpdate /v ProductVersion /t REG_SZ /d "Windows 10" /f
reg add HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\WindowsUpdate /v TargetReleaseVersion /t REG_DWORD /d 1 /f
reg add HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\WindowsUpdate /v ProductVersion /t REG_SZ /d 21H2 /f
```

## ニュースと関心ごとを無効
```bat
reg add HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Feeds /v ShellFeedsTaskbarViewMode /t REG_DWORD /d 2 /f
```
