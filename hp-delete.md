## HP

![image](https://user-images.githubusercontent.com/1501327/160033928-316ece97-b5bd-478d-b306-db5c3cd4ec0d.png)

```bat
reg delete HKEY_CLASSES_ROOT\CLSID\{0DB64048-7207-4864-8417-D5E2A500423D}
```

```bat
sc config "HpTouchpointAnalyticsService" start= disabled
sc config "HPAppHelperCap" start= demand
sc config "HPDiagsCap" start= demand
sc config "LanWlanWwanSwitchingServiceDSU" start= demand
sc config "HotKeyServiceDSU" start= demand
sc config "HPNetworkCap" start= demand
sc config "HPSysInfoCap" start= demand

sc config "HP Comm Recover" start= demand
sc config "SecurityUpdateService" start= disabled
sc config "BrEndpointSvc" start= disabled
sc config "BrService" start= demand
sc config "BrRmService" start= demand
```


```
[HKEY_CLASSES_ROOT\CLSID\{0DB64048-7207-4864-8417-D5E2A500423D}]
@="HP Support Assistant Quick Access"

[HKEY_CLASSES_ROOT\CLSID\{0DB64048-7207-4864-8417-D5E2A500423D}\Implemented Categories]

[HKEY_CLASSES_ROOT\CLSID\{0DB64048-7207-4864-8417-D5E2A500423D}\Implemented Categories\{00021492-0000-0000-C000-000000000046}]

[HKEY_CLASSES_ROOT\CLSID\{0DB64048-7207-4864-8417-D5E2A500423D}\InprocServer32]
@="C:\\Program Files (x86)\\HP\\HP Support Framework\\Resources\\HPSFMessenger9_3\\HPSFTaskbar.dll"
"ThreadingModel"="Apartment"

```
