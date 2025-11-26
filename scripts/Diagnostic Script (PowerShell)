# PC Diagnostics Script
Write-Host "Running PC Diagnostics..." -ForegroundColor Cyan

# System Information
Write-Host "Collecting system information..."
systeminfo | Out-File -FilePath "system_info.txt"

# Disk Health
Write-Host "Checking disk health..."
Get-PhysicalDisk | Select-Object FriendlyName, HealthStatus, OperationalStatus | Out-File -Append "system_info.txt"

# Memory Usage
Write-Host "Checking memory usage..."
Get-CimInstance Win32_OperatingSystem | Select-Object FreePhysicalMemory, TotalVisibleMemorySize | Out-File -Append "system_info.txt"

# Network Connectivity
Write-Host "Testing network connectivity..."
test-NetConnection google.com -InformationLevel Detailed | Out-File -Append "system_info.txt"

Write-Host "Diagnostics Complete. Output saved to system_info.txt" -ForegroundColor Green