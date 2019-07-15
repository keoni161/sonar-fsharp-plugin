# SonarQube F# Code Analyzer Plugin

The plugin enables analysis of F# within SonarQube.

## Builds

[![Build status](https://ci.appveyor.com/api/projects/status/jira637y22trnuc4/branch/master?svg=true)](https://ci.appveyor.com/project/jorgecosta/sonar-fsharp-plugin-wxq94/branch/master)
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=jmecsoftware.sonarqube.fsharp%3Asonar-communityfsharp-analyzer&metric=alert_status)](https://sonarcloud.io/dashboard?id=jmecsoftware.sonarqube.fsharp%3Asonar-communityfsharp-analyzer)

Download latest snapshot from Appveyor: <https://ci.appveyor.com/project/jorgecosta/sonar-fsharp-plugin-wxq94/build/artifacts>

## Description / Features

- Metrics: LOC, number of classes, number of methods
- Code duplication detection
- FSharpLint Support
- Runs under windows and Linux (mono)

## Configuration

### Requirements

- Minimal supported version of SonarQube: 6.7 LTS

### Installation

- Download the JAR plugin file from releases and copy it to the _extensions/plugins/_
directory of your SonarQube installation then start server.
The file _logs/sonar.log_ will then contain a log line indicating the loaded
plugin or any errors. The installed plugin will also be shown
on the Marketplace of your SonarQube installation.
- Review the F# quality profile before running.

### General Configuration

- `sonar.fs.file.suffixes` - files extensions to import

### Coverage and Tests

Please use generic solutions like
<https://docs.sonarqube.org/latest/analysis/generic-test/> or
<https://github.com/jmecsoftware/sonarqube-testdata-plugin>
