# SNIG Search Services

Customized search for SNIG metadata

## Installing the module

### GeoNetwork version to use with this module

Use GeoNetwork 3.4+. It's not supported in older versions so don't plug it into it!

### Adding module to the source code

The best approach is to add the module as a submodule into GeoNetwork project root.

```
git submodule add -b 3.4.x https://gitlab.wkt.pt/snig/geonetwork/snig-services.git snig-services
```
Add module to pom.xml
```
<modules>
    ...
    <module>snig-services</module>
    ...
</modules>
```

Add the dependency in the web module in web/pom.xml:

```
<dependency>
  <groupId>${project.groupId}</groupId>
  <artifactId>snig-services</artifactId>
  <version>${project.version}</version>
</dependency>
```
