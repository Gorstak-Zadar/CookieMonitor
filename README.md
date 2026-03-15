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

---

## Disclaimer

**NO WARRANTY.** THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.

**Limitation of Liability.** IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
