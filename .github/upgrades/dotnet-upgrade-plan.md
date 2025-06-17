# .NET 8.0 Upgrade Plan

## Execution Steps

1. Validate that an .NET 8.0 SDK required for this upgrade is installed on the machine and if not, help to get it installed.
2. Ensure that the SDK version specified in global.json files is compatible with the .NET 8.0 upgrade.
3. Upgrade Runner.Service\Windows\RunnerService.csproj
4. Run unit tests to validate upgrade in the projects listed below:
  - Test\Test.csproj

## Settings

This section contains settings and data used by execution steps.

### Excluded projects

| Project name                                   | Description                 |
|:-----------------------------------------------|:---------------------------:|

### Aggregate NuGet packages modifications across all projects

### Project upgrade details

#### Runner.Service\Windows\RunnerService.csproj modifications

Project properties changes:
  - Project file needs to be converted to SDK-style
  - Target framework should be changed from `.NETFramework,Version=v4.8` to `net8.0-windows`

NuGet packages changes:
  - None

Other changes:
  - None
