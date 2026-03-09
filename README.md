# 🍪 CookieMonitor

> PowerShell utility to **backup**, **monitor**, and **reset** Chrome cookie databases — with scheduled tasks for logon, startup, and periodic checks.

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 📦 **Backup** | Backs up Chrome `Cookies` database to `%ProgramData%\CookieBackup` |
| 🔄 **Monitor** | Scheduled task runs every 5 minutes to detect changes |
| 🔐 **Password Reset** | Optional scheduled password reset on shutdown |
| 📝 **Logging** | Logs to `CookieMonitor.log`, `NewPassword.log`, `ScriptErrors.log` |
| ⏰ **Scheduled Tasks** | MonitorCookiesLogon, BackupCookiesOnStartup, MonitorCookies, ResetPasswordOnShutdown |

---

## 📋 Requirements

| Requirement | Details |
|-------------|---------|
| **OS** | Windows 10/11 |
| **PowerShell** | 5.1+ |
| **Chrome** | Default path `%LocalAppData%\Google\Chrome\User Data\Default\Cookies` |

---

## 🚀 Usage

```powershell
# Install and schedule (copy to C:\Windows\Setup\Scripts\Bin, register tasks)
.\CookieMonitor.ps1

# Run monitoring only
.\CookieMonitor.ps1 -Monitor

# Backup cookies
.\CookieMonitor.ps1 -Backup

# Reset password (scheduled)
.\CookieMonitor.ps1 -ResetPassword
```

---

<p align="center">
  <sub>🛡️ Gorstak Privacy Tooling</sub>
</p>
