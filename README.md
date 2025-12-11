# GitWrap

GitWrap is a PowerShell-first wrapper around `git.exe` and Azure DevOps operations.  
It provides typed cmdlets, consistent output, minimal console noise, and robust error handling — designed for automation and professional scripting workflows.

## Features

- Unified PowerShell API for Git commands  
- Strongly typed, predictable output objects  
- Centralized git invocation (no direct `git` calls in scripts)  
- Clean error handling and silent-by-default execution  
- Azure DevOps–friendly helpers (pipelines, artifacts, credentials)  
- Extensible structure for additional Git/AzDO tooling

## Installation

```powershell
# Development / local use
git clone https://github.com/<org>/GitWrap.git
Import-Module ./GitWrap/GitWrap.psd1
```

## Usage Example

```powershell
# Get current branch
Get-CurrentBranch

# List branches
Get-BranchList

# Retrieve DevOps credentials
Get-CmdkeyDevOps
```

## Project Structure

```
GitWrap/
  GitWrap.psd1
  GitWrap.psm1
  GitWrap_Header.ps1
  GitWrap.Format.ps1xml
  Public/
  Private/
  Types/
```

## Contributing

Pull requests are welcome.  
Please follow the existing patterns: typed output, clean error handling, no direct calls to `git`, and minimal console noise.

## License

MIT License (or update to your preferred license).
