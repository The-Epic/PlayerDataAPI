## Dependency
```xml
<repository>
  <id>jeff-media-public</id>
  <name>JEFF Media GbR Repository</name>
  <url>https://repo.jeff-media.com/public</url>
</repository>
<dependency>
  <groupId>com.jeff_media.playerdatapi</groupId>
  <artifactId>playerdataapi-dist</artifactId>
  <version>1.0-SNAPSHOT</version>
  <scope>provided</scope>
</dependency>
```

## Usage
1. Depend on "PlayerDataAPI"
2. Get the API through the Plugin Manager, and cast it to PlayerDataAPI

### Spigot
```java
PlayerDataAPI playerDataAPI = (PlayerDataAPI) Bukkit.getPluginManager().getPlugin("PlayerDataAPI");
DataProvider provider = playerDataAPI.getProvider();
```

### BungeeCord
```java
PlayerDataAPI playerDataApi = (PlayerDataAPI) ProxyServer.getInstance().getPluginManager().getPlugin("PlayerDataAPI");
DataProvider provider = playerDataApi.getProvider();
```