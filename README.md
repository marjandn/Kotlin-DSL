# Kotlin-DSL :heart_eyes:

## Migrating build logic from Groovy to Kotlin

Gradle 5.0 has been released with lots of features and especially with the support of production-ready Kotlin DSL 


- **STEP 1 :**

Update to ``Gradle Wrapper 5.0`` or higher


- **STEP 2 :**

Fix ALL ``String quotes -> single quotes to double quotes `` ***CTRL+ SHIFT + R***

⚠️ Dont forget the ``settings.gradle`` file

- **STEP 3 :**

change all space to ``() or = ()`` -> ``function () / property =``


- **STEP 4 :** 


``apply plugin: "com.android.application" to plugins {
    id("com.android.application")
    }``
    


- **STEP 5 :**

Conversion ->  rename ``build.gradle`` files from ``xx.gradle`` to ``xx.gradle.kts``  -> ``settings.gradle`` files to ``settings.gradle.kts ``




- **STEP 6 :**

change ``release`` to ``getByName(String)`` 

``minifyEnabled`` to ``isMinifyEnabled`` 

``fileTree`` to ``fileTree(Map<String, ?> args)``



- **STEP 7 :**  :point_left:

create ``buildSrc`` dir -> ``build.gradle.kts ``


***migrate from groovy to Kotlin DSL DONE !*** :grin: 


