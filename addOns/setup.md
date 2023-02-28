## Instruction to setup on local
* Apache ant Installation [reference link](https://ant.apache.org/manual/install.html)
* Add changes for mirroring in `~./m2/settings.xml` and same changes in `/opt/apache-maven-2.2.1/conf/settings.xml` since maven repo supports only https.
```
<settings>
  <mirrors>
    <mirror>
      <id>other-mirror</id>
      <name>Other Mirror Repository</name>
      <url>https://repo1.maven.org/maven2/</url>
      <mirrorOf>central</mirrorOf>
    </mirror>
  </mirrors>
</settings>
```
* Change `kite-morphlines-core` version to `0.15.0` in `lucene-solr/lucene/ivy-versions.properties`.