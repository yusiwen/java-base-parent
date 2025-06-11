# Parent POM for Java Projects

[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg)](https://www.apache.org/licenses/LICENSE-2.0.html)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/yusiwen/java-base-parent/graphs/commit-activity)
[![GitHub tag](https://img.shields.io/github/v/tag/yusiwen/java-base-parent.svg)](https://GitHub.com/yusiwen/java-base-parent/tags/)
[![Maven Central](https://img.shields.io/maven-central/v/cn.yusiwen/java-base-parent)](https://central.sonatype.com/artifact/cn.yusiwen/java-base-parent)

Parent POM for my Java porjects.

## Usage

Set project's parent to `cn.yusiwen:java-base-parent`

```xml
<parent>
  <groupId>cn.yusiwen</groupId>
  <artifactId>java-base-parent</artifactId>
  <version>{LATEST_RELEASE}</version>
</parent>
```

## Plugins

Code Analysis:

- [Error Prone](https://errorprone.info/index)
- [Modernizer Maven Plugin](https://github.com/gaul/modernizer-maven-plugin)
- [Apache Maven Checkstyle Plugin](https://maven.apache.org/plugins/maven-checkstyle-plugin/): Default [checkstyle.xml](https://github.com/yusiwen/maven-build-helper/blob/master/src/main/resources/checkstyle.xml) is injected by [cn.yusiwen:maven-build-helper](https://github.com/yusiwen/maven-build-helper)
- [SpotBugs Maven Plugin](https://spotbugs.github.io/spotbugs-maven-plugin/)
  - [mebigfatguy/fb-contrib](https://github.com/mebigfatguy/fb-contrib)
  - [find-sec-bugs/find-sec-bugs](https://github.com/find-sec-bugs/find-sec-bugs)
  - [KengoTODA/findbugs-slf4j](https://github.com/KengoTODA/findbugs-slf4j)
- [Maven Enforcer Plugin](https://maven.apache.org/enforcer/maven-enforcer-plugin/)
- [Apache Maven PMD Plugin](https://maven.apache.org/plugins/maven-pmd-plugin/)
- [Alibaba Java Coding Guidelines](https://github.com/alibaba/p3c)
- [SonarQube Scanner for Maven](https://github.com/SonarSource/sonar-scanner-maven)
- [OWASP Dependency Check Plugin](https://jeremylong.github.io/DependencyCheck/dependency-check-maven/)
  
Code Formatter:

- [Formatter Maven Plugin](https://code.revelc.net/formatter-maven-plugin/): Default indent is 4 spaces, configred by [this file](https://github.com/yusiwen/maven-build-helper/blob/master/src/main/resources/formatter-4spaces.xml) (injected by [cn.yusiwen:maven-build-helper](https://github.com/yusiwen/maven-build-helper))
- [ImpSort Maven Plugin](https://code.revelc.net/impsort-maven-plugin/)
- [Tidy Maven Plugin](https://www.mojohaus.org/tidy-maven-plugin/)
- [whitespace-maven-plugin](https://github.com/yusiwen/whitespace-maven-plugin)
- [acegi/xml-format-maven-plugin](https://github.com/acegi/xml-format-maven-plugin)

Building:

- [Apache Maven Compiler Plugin](https://maven.apache.org/plugins/maven-compiler-plugin/)
- [Apache Maven Resources Plugin](https://maven.apache.org/plugins/maven-resources-plugin/)
- [Apache Maven Source Plugin](https://maven.apache.org/plugins/maven-source-plugin/)
- [Apache Maven AntRun Plugin](https://maven.apache.org/plugins/maven-antrun-plugin/)
- [fabric8io/docker-maven-plugin](https://github.com/fabric8io/docker-maven-plugin)
- [git-commit-id/git-commit-id-maven-plugin](https://github.com/git-commit-id/git-commit-id-maven-plugin)
- [Git Build Hook Maven Plugin](https://github.com/rudikershaw/git-build-hook)
- [Apache Maven JAR Plugin](https://maven.apache.org/plugins/maven-jar-plugin/)
- [Apache Maven WAR Plugin](https://maven.apache.org/plugins/maven-war-plugin/)
- [Apache Maven Clean Plugin](https://maven.apache.org/plugins/maven-clean-plugin/)
- [Apache Maven Javadoc Plugin](https://maven.apache.org/plugins/maven-javadoc-plugin/)
- [Maven HTMLCompressor Plugin](https://github.com/alextunyk/htmlcompressor-maven-plugin)
- [YUI Compressor Maven Mojo](http://davidb.github.io/yuicompressor-maven-plugin/)

Site and Report:

- [Maven Doxia](https://maven.apache.org/doxia/)
- [Apache Maven Fluido Skin](https://maven.apache.org/skins/maven-fluido-skin/)
- [Apache Maven Changelog Plugin](https://maven.apache.org/plugins/maven-changelog-plugin/)
- [Apache Maven Changes Plugin](https://maven.apache.org/plugins/maven-changes-plugin/index.html)
- [Maven 2 JavaNCSS Plugin](https://www.mojohaus.org/javancss-maven-plugin/)
- [JDepend Maven Plugin](https://www.mojohaus.org/jdepend-maven-plugin/)
- [Maven JXR Plugin](https://maven.apache.org/jxr/maven-jxr-plugin/)
- [Apache Maven Project Info Reports Plugin](https://maven.apache.org/plugins/maven-project-info-reports-plugin/)
- [Taglist Maven Plugin](https://www.mojohaus.org/taglist-maven-plugin/)
- [Versions Maven Plugin](https://www.mojohaus.org/versions-maven-plugin/)

Release and Deploy:

- [Maven Release Plugin](https://maven.apache.org/maven-release/maven-release-plugin/index.html)
- [Apache Maven Deploy Plugin](https://maven.apache.org/plugins/maven-deploy-plugin/)
- [Apache Maven GPG Plugin](https://maven.apache.org/plugins/maven-gpg-plugin/)
- [License Maven Plugin](https://www.mojohaus.org/license-maven-plugin/)
  - [license-maven-plugin-git](https://github.com/mathieucarbou/license-maven-plugin/tree/master/license-maven-plugin-git)
- [Wagon Maven Plugin](https://www.mojohaus.org/wagon-maven-plugin/)
  - [wagon-git](https://mvnrepository.com/artifact/net.trajano.wagon/wagon-git)
  - [Maven Wagon SSH](https://maven.apache.org/wagon/wagon-providers/wagon-ssh/)

Miscellaneous:

- [Properties Maven Plugin](https://www.mojohaus.org/properties-maven-plugin/)
- [Animal Sniffer](https://www.mojohaus.org/animal-sniffer/)
- [jdcasey/directory-maven-plugin](https://github.com/jdcasey/directory-maven-plugin)
- [Exec Maven Plugin](https://www.mojohaus.org/exec-maven-plugin/)
- [Apache Maven Dependency Plugin](https://maven.apache.org/plugins/maven-dependency-plugin/)
- [Flyway Maven Plugin](https://flywaydb.org/documentation/usage/maven/)
- [Spring Boot Maven Plugin](https://docs.spring.io/spring-boot/docs/current/maven-plugin/reference/htmlsingle/)

## Default Project Dependencies

- [com.github.spotbugs:spotbugs-annotations](https://mvnrepository.com/artifact/com.github.spotbugs/spotbugs-annotations)
- [org.gaul:modernizer-maven-annotations](https://mvnrepository.com/artifact/org.gaul/modernizer-maven-annotations)
- [org.projectlombok:lombok](https://mvnrepository.com/artifact/org.projectlombok/lombok)

## Profiles

- `jar`: Default profile, build jar and skip docker image building
- `docker`: Build jar and docker image
- `release`: Release project to remote repository
- `compression`: Compress html/css/js files, automatically activated when `.compress` file is found
- `format`: Format all project files, automatically activated when `.format` file is found
- `sort`: Tidy pom.xml
- `jdk8`: Set maven plugins version compatible with JDK8, automatically activated when JDK8 is used
- `jdk9+`: Set JDK9+ compatibility, automatically activated when JDK9+ is used
- `error-prone-common`: Import `error_prone_annotations` dependency, automatically activated when `.error-prone` file is found
- `jdk8-error-prone`: Set error prone in JDK8 environment, automatically activated when JDK8 is used
- `jdk9-error-prone`: Set error prone in JDK9+ environment, automatically activated when JDK9+ is used
- `jdk16-error-prone`: Set error prone in JDK16 environment, automatically activated when JDK16+ is used
- `eclipse`: Set m2e configuration, automatically activated when `m2e.version` is set
