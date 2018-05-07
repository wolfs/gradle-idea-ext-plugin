# gradle-idea-ext-plugin

[![JetBrains team project](http://jb.gg/badges/team.svg)](https://confluence.jetbrains.com/display/ALL/JetBrains+on+GitHub)

Proof-of-concept plugin to store arbitrary IJ settings in gradle script

### How to build

as simple as

    ./gradlew build

### How to apply

Apply from Gradle plugin repository

    plugins {
      id "org.jetbrains.gradle.plugin.idea-ext" version "0.1"
    }

Or build and drop resulting jar into root directory of a project and add following snippet to `build.grade`

    buildscript {
      dependencies {
        classpath files('gradle-idea-ext.jar')
      }
    }
    apply plugin: 'org.jetbrains.gradle.plugin.idea-ext'

      
