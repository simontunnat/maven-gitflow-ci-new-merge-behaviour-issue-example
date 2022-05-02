# Maven Git-Flow Plugin New Merge Behaviour Issue Example
[![Build](https://github.com/simontunnat/maven-gitflow-ci-new-merge-behaviour-issue-example/workflows/CI/badge.svg)](https://github.com/simontunnat/maven-parent/actions?query=workflow%3ACI)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

This is an example for issue [https://github.com/aleksandr-m/gitflow-maven-plugin/issues/345](#345) of the Git-Flow Maven plugin.

## Requirements
* Java Version 8 or later (the project is build against JDK 8, 11 and 16)

## Usage
Execute the following command to start the release:
```
mvn clean gitflow:release-start -B -DcommitDevelopmentVersionAtStart -DuseSnapshotInRelease
```

Execute the following command to finish the release:
```
mvn clean gitflow:release-finish -B -DcommitDevelopmentVersionAtStart -DuseSnapshotInRelease -DpushRemote=false
```

## Legal
Copyright 2022 Simon Tunnat

Licensed under the [Apache License](LICENSE), Version 2.0.
