Check out ObjectBox
===================

Looking for object persistence faster than SQLite? Check out our new mobile database [ObjectBox](https://objectbox.io/) ([GitHub](https://github.com/objectbox/objectbox-java)). 

greenDAO
========
greenDAO is a light & fast ORM for Android that maps objects to SQLite databases. Being highly optimized for Android, greenDAO offers great performance and consumes minimal memory.

**<font size="+1">Home page, documentation, and support links: http://greenrobot.org/greendao/</font>**

[![Build Status](https://travis-ci.org/greenrobot/greenDAO.svg?branch=master)](https://travis-ci.org/greenrobot/greenDAO)

Features
--------
greenDAO's unique set of features:

* Rock solid: greenDAO has been around since 2011 and is used by countless famous apps
* Super simple: concise and straight-forward API, in V3 with annotations
* Small: The library is <150K and it's just plain Java jar (no CPU dependent native parts)
* Fast: Probably the fastest ORM for Android, driven by intelligent code generation
* Safe and expressive query API: QueryBuilder uses property constants to avoid typos
* Powerful joins: query across entities and even chain joins for complex relations
* Flexible property types: use custom classes or enums to represent data in your entity
* Encryption: supports SQLCipher encrypted databases

Add greenDAO to your project
----------------------------
greenDAO is available on Maven Central. Please ensure that you are using the latest versions of the [greendao](https://search.maven.org/search?q=g:org.greenrobot%20AND%20a:greendao) and [greendao-gradle-plugin](https://search.maven.org/search?q=g:org.greenrobot%20AND%20a:greendao-gradle-plugin) artifact.

Add the following Gradle configuration to your Android project. In your root `build.gradle` file:
```groovy
buildscript {
    repositories {
        jcenter()
        mavenCentral() // add repository
    }
    dependencies {
        classpath 'com.android.tools.build:gradle:3.1.1'
        classpath 'org.greenrobot:greendao-gradle-plugin:3.2.2' // add plugin
    }
}
```
In your app modules `app/build.gradle` file:
```groovy
apply plugin: 'com.android.application'
apply plugin: 'org.greenrobot.greendao' // apply plugin
 
dependencies {
    implementation 'org.greenrobot:greendao:3.2.2' // add library
}
```

Note that this hooks up the greenDAO Gradle plugin to your build process. When you build your project, it generates classes like DaoMaster, DaoSession and DAOs.

Continue at the [Getting Started](http://greenrobot.org/greendao/documentation/how-to-get-started/) page.

Homepage, Documentation, Links
------------------------------
For more details on greenDAO please check [greenDAO's website](http://greenrobot.org/greendao). Here are some direct links you may find useful:

[Features](http://greenrobot.org/greendao/features/)

[Getting Started](http://greenrobot.org/greendao/documentation/how-to-get-started/)

[Documentation](http://greenrobot.org/greendao/documentation/)

[Changelog](http://greenrobot.org/greendao/changelog/)

[Technical FAQ](http://greenrobot.org/greendao/documentation/technical-faq/) (incl. ProGuard rules)

[Non-Technical FAQ](http://greenrobot.org/greendao/documentation/faq/)

[Migrating to greenDAO 3](http://greenrobot.org/greendao/documentation/updating-to-greendao-3-and-annotations/)

More Open Source by greenrobot
==============================
[__ObjectBox__](https://github.com/objectbox/objectbox-java) is a new superfast object-oriented database for mobile.

[__EventBus__](https://github.com/greenrobot/EventBus) is a central publish/subscribe bus for Android with optional delivery threads, priorities, and sticky events. A great tool to decouple components (e.g. Activities, Fragments, logic components) from each other.

[__Essentials__](https://github.com/greenrobot/essentials) is a set of utility classes and hash functions for Android & Java projects.
