## HP

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
```
