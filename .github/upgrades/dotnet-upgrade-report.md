# .NET 8 Upgrade Report

## Project modifications

| Project name                                 | Old Target Framework    | New Target Framework   | Commits                                   |
|:---------------------------------------------|:-----------------------:|:----------------------:|:-------------------------------------------|
| Runner.Service\Windows\RunnerService.csproj  | .NETFramework,Version=v4.8 | net8.0-windows         | 86123eb3, 23d09b92, 01380e61               |

## NuGet Packages

_No NuGet package upgrades were performed during this upgrade._

## All commits

| Commit ID  | Description                                                                 |
|:-----------|:----------------------------------------------------------------------------|
| 86123eb3   | commit upgrade plan                                                         |
| 23d09b92   | Remove unused references from RunnerService.csproj                           |
| 01380e61   | Remove AssemblyInfo.cs and update RunnerService.csproj                       |

## Test Results

- Test project: Test\Test.csproj
- 657 tests passed, 29 tests failed, 0 skipped

## Next steps

- Review and address the 29 failed unit tests in Test\Test.csproj to ensure full compatibility after the upgrade.
- Run formatting and additional validation as needed.
