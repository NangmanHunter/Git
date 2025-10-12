## CreateGitKeep
```ps1
$rootPath = Get-Location

# 재귀적으로 각 폴더 검사
function Check-FolderFiles {
    param([string]$Path)

    # 현재 폴더의 파일만 검사
    $files = Get-ChildItem -Path $Path -File -Force -ErrorAction SilentlyContinue

    if ($files) {
        Write-Host "✅ExistFile🚥📁📄CheckDirectory: $Path"
    } else {
        Write-Host "❌ExistFile🚥📁📭CheckDirectory: $Path"
        ni -Path "${Path}\.gitkeep"
    }

    # 하위 폴더가 있으면 재귀 호출
    $subDirs = Get-ChildItem -Path $Path -Directory -Force -ErrorAction SilentlyContinue
    foreach ($dir in $subDirs) {
        Check-FolderFiles -Path $dir.FullName
    }
}

# 시작
Check-FolderFiles -Path $rootPath
```
