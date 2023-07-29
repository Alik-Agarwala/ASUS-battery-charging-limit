## 🔋 ASUS BATTERY CHARGING LIMIT

#### This script is used to set the charging limit for ASUS laptops (tested with ASUS ZenBook 14 UX425EA).

### For Linux 🐧:

`Step 1:` Download the [asus-battery-health-charging.sh](https://github.com/alik-agarwala/ASUS-battery-charging-limit/blob/main/asus-battery-health-charging.sh) script.

`Step 2:` Grant executable permission to the script file.
```bash
  chmod +x asus-battery-health-charging.sh
```

`Step 3:` Execute the script, passing the desired charging limit value (1 - 100) as a command-line argument.
```bash
  sudo sh asus-battery-health-charging.sh 60
```
`Note:` This will set the battery charging limit to 60%. The setting will persist even after restarting. To change the limit, follow Step 3 and pass the desired value.

---

### For Windows 🪟:

#### Please run PowerShell with Administrator priviledges.

`Step 1:` Download the [asus-battery-health-charging.ps1](/asus-battery-health-charging.ps1) script.

`Step 2:` Grant executable permission to the script file. (Press Y upon prompt).
```powershell
  Set-ExecutionPolicy RemoteSigned
```

`Step 3:` Execute the script, passing the desired charging limit value (1 - 100) upon prompt.
```powershell
  ./asus-battery-health-charging.ps1
```

`Alternate Step:` if you have difficulty running the script, simple copy the code to administrator PowerShell and set the limit.

`Note:`  The setting will persist even after restarting. To change the limit, follow Step 3 and pass the desired value. If you wan to check limit status:
```powershell
  powercfg -q 381b4222-f694-41f0-9685-ff5bb260df2e SUB_BATTERY
```

---

[![forthebadge](https://forthebadge.com/images/badges/60-percent-of-the-time-works-every-time.svg)](https://forthebadge.com)
