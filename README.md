# Custom Maven Plugin

Just a basic demo of a custom maven plugin

## Usage
To use just run `mvn install` and now that you have it installed in your local m2 repostory you can
include it into any project with plugin configuration added to your `pom.xml`:

```
<build>
    <plugins>
        <plugin>
            <groupId>com.asgarov</groupId>
            <artifactId>custom_maven_plugin</artifactId>
            <version>1.0-SNAPSHOT</version>
            <executions>
                <execution>
                    <phase>compile</phase>
                    <goals>
                        <goal>custom</goal>
                    </goals>
                </execution>
            </executions>
        </plugin>
    </plugins>
</build>
```