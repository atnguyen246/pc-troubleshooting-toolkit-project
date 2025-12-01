# User Issue Logger Script
# Saves IT support issues to a log file with timestamps

# Set log file path (change if needed)
$logFile = "C:\IT_Logs\User_Issue_Log.csv"

# Create log file with headers if it doesn't exist
if (-not (Test-Path $logFile)) {
    "Date,Technician,User,Issue Description,Status" | Out-File -FilePath $logFile -Encoding UTF8
}

Write-Host "=== User Issue Logger ===" -ForegroundColor Cyan

# Collect input
$technician   = Read-Host "Enter your name"
$user         = Read-Host "Enter the user's name"
$issue        = Read-Host "Describe the issue"
$status       = Read-Host "Current status (e.g., Open, In Progress, Resolved)"

# Timestamp
$date = Get-Date -Format "yyyy-MM-dd HH:mm:ss"

# Create log entry
$entry = "$date,$technician,$user,$issue,$status"

# Append to log file
Add-Content -Path $logFile -Value $entry

Write-Host "`nIssue logged successfully!" -ForegroundColor Green
Write-Host "Log saved to: $logFile"
