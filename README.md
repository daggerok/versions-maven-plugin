# versions-maven-plugin
Check for new dependency updates

suppose you have in your `pom.xml` file:

```xml
<project>
  </build>
    <plugins>
      <plugin>
        <groupId>org.codehaus.mojo</groupId>
        <artifactId>versions-maven-plugin</artifactId>
        <version>2.7</version>
        <configuration>
          <generateBackupPoms>false</generateBackupPoms>
          <allowSnapshots>true</allowSnapshots>
          <allowIncrementalUpdates>true</allowIncrementalUpdates>
          <excludeReactor>false</excludeReactor>
        </configuration>
      </plugin>
    </plugins>
  </build>
</project>
```

then run command to check for new dependency versions update:

```bash
mvn versions:display-dependency-updates
```

see reference [documentation](https://www.mojohaus.org/versions-maven-plugin/examples/display-dependency-updates.html)
