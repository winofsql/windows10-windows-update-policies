## セキュリティ

```reg
reg add HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Google\Chrome /v ShowHomeButton /t REG_DWORD /d 1 /f
reg add HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Google\Chrome /v PasswordManagerEnabled /t REG_DWORD /d 0 /f
reg add HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Google\Chrome /v AutofillCreditCardEnabled /t REG_DWORD /d 0 /f
reg add HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Google\Chrome /v AutofillAddressEnabled /t REG_DWORD /d 0 /f
```
