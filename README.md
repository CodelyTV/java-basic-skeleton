# Java Bootstrap (base / project skeleton)

## Introduction

This is a repository intended to serve as a starting point if you want to bootstrap a project in Java with JUnit and Gradle

## How To Start

1. Install Java: `brew cask install java`
2. Clone this repository: `git clone https://github.com/CodelyTV/java-bootstrap`.
3. Execute some [Gradle lifecycle tasks](https://docs.gradle.org/current/userguide/java_plugin.html#lifecycle_tasks) in order to check everything is OK:
    1. Create [the project JAR](https://docs.gradle.org/current/userguide/java_plugin.html#sec:jar) and other project artifacts:
    `./gradlew assemble --warning-mode all`
    2. Run the tests and plugins verification tasks:
    `./gradlew check --warning-mode all`
4. Start developing!

## How to update dependencies

* Gradle (current version: 5.1.1 - [releases](https://gradle.org/releases/)):
`./gradlew wrapper --gradle-version=5.1.1 --distribution-type=bin` or modifying the [gradle-wrapper.properties](gradle/wrapper/gradle-wrapper.properties#L3)
* JUnit (current version: 5.3.2 - [releases](https://junit.org/junit5/docs/snapshot/release-notes/index.html)):
[`build.gradle:11`](build.gradle#L11-L12)
