# CoApp scripts for CEF via NuGET

Use this package to create NuGet packages that add CEF to your
Visual Studio projects!

## Updating CEF version.
First, download new binary packages from LibCEF website.
```bash
$ vi luajit.autopkg  # change version and directories defines to match
$ git commit -m "Updated libCEF version to vX.XXXX.XXXX"
```

## Building CEF NuGet packages.
In Powershell
```bash
> Write-NuGetPackage .\cef.autopkg
```

## Installing CoApp NuGet helper scripts.
In administrator PowerShell:
```
> Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
```

In normal PowerShell:
```
> Update-CoAppTools -KillPowershells
```
