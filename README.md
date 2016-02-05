Mybatis Generator Plugin
======================================

[![Build Status](https://travis-ci.org/liebe444ever/mybatis-generator-plugin.svg?branch=master)](https://travis-ci.org/liebe444ever/mybatis-generator-plugin)

## Usage 

In your ```build.gradle``` file, add following plugin:

``` groovy
buildscript {
  repositories {
    maven {
      url "https://plugins.gradle.org/m2/"
    }
  }
  dependencies {
    classpath "gradle.plugin.com.arenagod.gradle:mybatis-generator-plugin:1.3"
  }
}

apply plugin: "com.arenagod.gradle.MybatisGenerator"

configurations {
    mybatisGenerator
}

mybatisGenerator {
    verbose = true
    configFile = 'src/main/resources/autogen/generatorConfig.xml'
}
```
