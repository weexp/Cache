[![Build Status](https://travis-ci.org/barakb/Cache.svg?branch=master)](https://travis-ci.org/barakb/Cache) 

Cache -- An LRU Java Cache
==========================

## DESCRIPTION

Fast Flexible efficient in memory LRU Java cache
This repository has the sources to [my post](http://bar-orion.blogspot.com/2012/02/fast-flexible-efficient-in-memory-java.html).

Barak.

Sample Usage:

```java
    Cache<String, byte[]> fileContentCache =
            new Cache<>(key -> readFileContent(new File(key)), 10);
```                    

See [example](https://github.com/barakb/Cache/blob/master/src/test/java/org/async/utils/cache/FileContentCache.java)


Maven dependency

```xml
    <dependency>
        <groupId>com.github.barakb</groupId>
        <artifactId>concurrent-cache</artifactId>
        <version>1.0</version>
    </dependency>
```