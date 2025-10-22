# Game Performance

## Game Settings

If your game is struggling, try:

- Turning down ==Render Distance==
- Look into ==JVM args== (see next section)
- Giving it some more ==RAM==——but not so much GC pauses noticeably lengthen.

## Java and the JVM

### Which Java to Use?

_Adoptium_ is nice; really, any OpenJDK build provider should be fine.

- [Adoptium Java 21](https://adoptium.net/?variant=openjdk21&jvmVariant=hotspott): for MC 1.20.5 or later, and [***Craftoria***](../modpacks/Craftoria) and [***All of Fabric 7***](../modpacks/aof7).

- [Adoptium Java 17](https://adoptium.net/?variant=openjdk17&jvmVariant=hotspot): for MC 1.17–1.20.4; and ***All of Fabric*** [**5**](../modpacks/aof5), [**6**](../modpacks/aof6), and [**7**](../modpacks/aof7).


### Java and Minecraft versions, and our Modpacks

| AOE Pack | Minecraft version | Java version (tied to MC version) |
|:-:|:-:|-|
| ***Craftoria*** | 1.21 | Java21 (runs better on Java25) |
| **AOF 7** | 1.20 | Java17 (runs better on Java21) |
| **AOF 6** | 1.19 | Java17 |
| **AOF 5** | 1.18 | Java17 |
| **AOF 4** | 1.17 | Java17 |
| **AOF 3** | 1.16 | Java8  |

### Java Args

#### For Clients

Around 6–8GB should work well for any AOE modpacks.

| AOE Mod Pack   | Java Args for Client           |
|:--------------:|--------------------------------|
| ***Craftoria***|`-XX:+UseZGC -XX:+ZGenerational` (Java25: `-XX:+UseZGC -XX:+UseCompactObjectHeaders`)|
| **AOF 7**      |`-XX:+UseZGC -XX:+ZGenerational` (only for Java21)|

These args do the following:
- `-XX:+UseZGC`: Enables the Z Garbage Collector
- `-XX:+ZGenerational`: Enables Generational Mode for ZGC - not needed on Java25, as it is now default
- `-XX:+UseCompactObjectHeaders`: Changes how the JVM stores objects in RAM, reducing memory usage (requires Java25)

#### For Servers

On a server GC through-put may be more valuable than latency—which the default `G1GC` garbage-collector will deliver. It is recommended to add its arg, `-XX:+UseG1GC`, for redundancy's sake.

---
