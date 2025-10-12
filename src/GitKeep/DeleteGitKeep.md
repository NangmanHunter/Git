## DeleteGitKeep
```ps1
$path = "C:\github-nangmanhunter\test"
$extension = ".gitkeep"

$files = Get-ChildItem -Path $path -File -Filter $extension -Recurse -Force -ErrorAction SilentlyContinue

foreach ($file in $files) {
    Remove-Item $file.FullName
    Write-Host "❌DeleteGitKeep: $($file.FullName)"
}
```