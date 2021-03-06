---
layout: post
title: "Apache Maven Plugin Tools Version 3.5.1 Released"
date: 2018-01-22 22:45:00
comments: true
categories: [Neuigkeiten,BM,Maven,Maven-Plugins,Maven-Plugin-Releases]
---
The Apache Maven team is pleased to announce the release of the 
[Apache Maven Plugin Tools, version 3.5.1](http://maven.apache.org/plugin-tools/).

The Maven Plugin Tools contains the necessary tools to generate  
rebarbative content like descriptor, help and documentation. In addition,  
it provides tools to write Maven Plugins in scripting languages like Ant  
or Beanshell.

The Maven Plugin Plugin is used to create a Maven plugin descriptor for  
any Mojo's found in the source tree, to include in the JAR. It is also  
used to generate report files for the Mojos as well as for updating the  
plugin registry, the artifact metadata and generating a generic help goal.

 * https://maven.apache.org/plugin-tools/
 * https://maven.apache.org/plugin-tools/maven-plugin-plugin/

You should specify the version in your project's plugin configuration:

``` xml
<plugin>
  <groupId>org.apache.maven.plugins</groupId>
  <artifactId>maven-plugin-plugin</artifactId>
  <version>3.5.1</version>
</plugin>
```
You can download the appropriate sources etc. from the [download page](https://maven.apache.org/plugins-tools/download.cgi).

<!-- more -->

[Release Notes - Maven Plugin Tools - Version 3.5.1](https://issues.apache.org/jira/secure/ReleaseNote.jspa?projectId=12317820&version=12338196)


Bugs:

 * {%ajl MPLUGIN-290 %} - Version 3.4 fails to parse enums with Regex patterns
 * {%ajl MPLUGIN-293 %} - Missing explanation on <requirements> on report goal
 * {%ajl MPLUGIN-314 %} - invalid requirement role generated in plugin.xml
 * {%ajl MPLUGIN-320 %} - JavaJavadocMojoDescriptorExtractor fails with Java 8 lambdas.
 * {%ajl MPLUGIN-322 %} - The javadoc for the @Parameter annotation should clearly state that those are only evaluated on fields of a Mojo
 * {%ajl MPLUGIN-324 %} - javadoc generated by helpmojo goal of maven-plugin-plugin produces build failures
 * {%ajl MPLUGIN-325 %} - Documentation incorrectly claims plugin:updateRegistry is bound to install phase
 * {%ajl MPLUGIN-328 %} - ArrayIndexOutOfBoundsException: 48188 
 * {%ajl MPLUGIN-330 %} - If and else-if branches has the same condition

Improvements:

 * {%ajl MPLUGIN-315 %} - improve mojo description: show parameter name as <parameter>
 * {%ajl MPLUGIN-319 %} - @since values ignored in report
 * {%ajl MPLUGIN-321 %} - improve documentation on maven-plugin-annotations telling that optional=true is sufficient
 * {%ajl MPLUGIN-326 %} - Remove timestamp in generated descriptor

Tasks:

 * {%ajl MPLUGIN-327 %} - switch to Git
 * {%ajl MPLUGIN-331 %} - Check the existence of plugin.xml rather than project packaging in PluginReport.canGenerateReport()


Enjoy,

-The Apache Maven team

