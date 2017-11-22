# simple_kotlin
# Very Simple Kotlin-App

Simplest Kotlin Application i could imagine.

## Building and Executing

Compiling is as simple as in java `kotlinc simple.kt`.
The result is `SimpleKt.class` - perfect java bytecode :-)

## Executing

* First and most obvious choice is running it as kotlin app:
```
$> kotlin SimpleKt
Hallo
```

* Since the kotlin compiler produces perfectly valid bytecode we could execute
this as java application.
Kotlins paradigm is KISS:
```
$> kotlinc simple.kt -include-runtime -d simple.jar
$> java -jar simple.jar
Hallo
```

* In case you don't hava java >= 8 installed docker to the rescue:
```bash
$ docker run --rm -v "$PWD":/tmp  -w /tmp java:openjdk-8-jre  java -jar simple.jar
Hallo
```
# EOF

