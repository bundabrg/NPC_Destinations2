# Craftbukkit and Maven

CraftBukkit jars must be added to your local maven repo before this will compile.

To do this follow these steps:

1. Compile the following CraftBukkit versions to produce the following files:
    - 1.8.8-R0.1-SNAPSHOT - craftbukkit-1.8.8.jar
    - 1.9.2-R0.1-SNAPSHOT - craftbukkit-1.9.2.jar
    - 1.9.4-R0.1-SNAPSHOT - craftbukkit-1.9.4.jar
    - 1.10.2-R0.1-SNAPSHOT - craftbukkit-1.10.2.jar
    - 1.11.2-R0.1-SNAPSHOT - craftbukkit-1.11.2.jar
    - 1.12.2-R0.1-SNAPSHOT - craftbukkit-1.12.2.jar

2. Copy all these files into a single directory and go into that directory

3. Enter the following to install it into your local .m2 maven repo (you obviously need maven installed):

```
mvn install:install-file -Dfile=craftbukkit-1.8.8.jar -DgroupId=org.bukkit -DartifactId=craftbukkit -Dversion=1.8.8-R0.1-SNAPSHOT -Dpackaging=jar
mvn install:install-file -Dfile=craftbukkit-1.9.2.jar -DgroupId=org.bukkit -DartifactId=craftbukkit -Dversion=1.9.2-R0.1-SNAPSHOT -Dpackaging=jar
mvn install:install-file -Dfile=craftbukkit-1.9.4.jar -DgroupId=org.bukkit -DartifactId=craftbukkit -Dversion=1.9.4-R0.1-SNAPSHOT -Dpackaging=jar
mvn install:install-file -Dfile=craftbukkit-1.10.2.jar -DgroupId=org.bukkit -DartifactId=craftbukkit -Dversion=1.10.2-R0.1-SNAPSHOT -Dpackaging=jar
mvn install:install-file -Dfile=craftbukkit-1.11.2.jar -DgroupId=org.bukkit -DartifactId=craftbukkit -Dversion=1.11.2-R0.1-SNAPSHOT -Dpackaging=jar
mvn install:install-file -Dfile=craftbukkit-1.12.2.jar -DgroupId=org.bukkit -DartifactId=craftbukkit -Dversion=1.12.2-R0.1-SNAPSHOT -Dpackaging=jar
```
