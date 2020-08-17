# FSharpLint Config Schema

JSON Schema for the FSharpLint configuration files

This repo includes:

- (WIP) JSON Schema generator (dotnet CLI tool)
- (WIP) VSCode extension for applying this JSON Schema
- (WIP) Configurations for deploying this JSON Schema on Netlify

## Setup

```bash
dotnet tool restore  # Install dotnet CLI tools
dotnet paket restore # Install dependencies
```

## JSON Schema generator

### Run

```bash
dotnet run -p src/FLConfigSchema
```

### Install

```bash
dotnet pack # Generate .nupkg file
dotnet tool install --add-source ./src/FLConfigSchema/nupkg fsharplint-config
```
