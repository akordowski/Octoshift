# Octoshift

[![CI](https://github.com/akordowski/Octoshift/actions/workflows/CI.yml/badge.svg)](https://github.com/akordowski/Octoshift/actions/workflows/CI.yml)

The purpose of this repository is to extract the code of the Octoshift library from the [gh-gei](https://github.com/github/gh-gei) (GitHub Enterprise Importer CLI) project and provide it as a NuGet packages. In this way the base code can be reused while creating custom migration extensions for the [GitHub CLI](https://github.com/cli/cli#installation).

## Usage

Add NuGet source

```pwsh
dotnet nuget add source https://nuget.pkg.github.com/akordowski/index.json `
  --name Octoshift  `
  --username USERNAME `
  --password TOKEN `
  --store-password-in-clear-text
```

Add NuGet package

```pwsh
dotnet add package Octoshift --source Octoshift
```
