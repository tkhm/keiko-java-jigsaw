# Keiko Java Jigsaw

Project Jigsaw: Quick Start Guide https://openjdk.java.net/projects/jigsaw/quick-start

JDK9 Jigsaw を試してみた - Qiita https://qiita.com/hashiwa/items/9ae1f8ad8d2e8f916664

Execute following commands on the caller directory:

```
javac -d mods/com.example.greetings ../jigsaw-sample/src/module-info.java ../jigsaw-sample/src/com/example/greetings/api/EnglishGreeting.java
javac --module-path mods -d mods/dev.tkhm.greetings src/module-info.java src/dev/tkhm/greetings/main/Main.java
java --module-path mods -m dev.tkhm.greetings/dev.tkhm.greetings.main.Main
```

Executed on the following env:

```
$java -version

openjdk version "11.0.2" 2019-01-15
OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.2+9)
OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.2+9, mixed mode)
```
