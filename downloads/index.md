---
layout: main
title: "Download IzPack"
---

<div class="page-header">
  <h1>Get IzPack</h1>
</div>

## Direct installer download

The current stable is release is **IzPack 4.3.5**.
We have relase candidates for the upcoming **IzPack 5.0**.

* [Download the installer for IzPack 5.0.0-rc4](http://dist.codehaus.org/izpack/releases/5.0.0-rc4/izpack-dist-5.0.0-rc4-installer.jar)
* [Download the installer for IzPack 4.3.5](http://dist.codehaus.org/izpack/releases/4.3.5/IzPack-install-4.3.5.jar)

Launching an IzPack-based installer is easy. On most operating systems, a double-click on the Jar file icon will do. Otherwise, you may need to launch it from a shell command:

    $ java -jar izpack-dist-5.0.0-rc4-installer.jar

If you are interested in the source code then please have a look at the [instructions for obtaining it from Git](/developers/).

## Maven users

For IzPack 4.3.5:

    <dependency>
        <groupId>org.codehaus.izpack</groupId>
        <artifactId>izpack-standalone-compiler</artifactId>
        <version>4.3.5</version>
    </dependency>

For IzPack 5.x:

    <dependency>
        <groupId>org.codehaus.izpack</groupId>
        <artifactId>izpack-maven-plugin</artifactId>
        <version>5.0.0-rc4</version>
    </dependency>

[See the new IzPack Maven plugin documentation](http://izpack.codehaus.org/izpack-maven-plugin/).

If you are migrating from IzPack 4 to IzPack 5, do not forget to [read our migration notes](http://docs.codehaus.org/display/IZPACK/Upgrading+Existing+Installers+from+IzPack+4.x+to+5.0).

## Gradle users

An independent and very promising project gives Gradle users a plugin for IzPack: [http://github.com/bmuschko/gradle-izpack-plugin](http://github.com/bmuschko/gradle-izpack-plugin)

## Scala SBT users

Brian Clapper develops an awesome plugin for Scala SBT: [http://software.clapper.org/sbt-izpack/](http://software.clapper.org/sbt-izpack/)

## Apache BuildR users

Niklaus Giger maintains a plug-in for [Apache BuildrR](http://buildr.apache.org/). The code can be found at [https://github.com/ngiger/buildrizpack](https://github.com/ngiger/buildrizpack).

* [RDoc](http://ngiger.dyndns.org/jenkins/job/buildrizpack/lastSuccessfulBuild/artifact/rdoc/README_rdoc.html)
* [Howto](https://cwiki.apache.org/confluence/display/BUILDR/How+to+build+an+IzPack+installer)

## Graphical user interfaces

<h3>DCP Setup Maker</h3>
[DCP Setup Maker](http://sourceforge.net/projects/devcompack) is an opensource project, powered by IzPack and developed by Said El Imam,
that generates java installers easily for a set of files, without the need of coding knowledge.
It automatically writes the xml code, and compiles it for you.

DCP Setup Maker is not affiliated with the IzPack project, and is released under the terms of the [Apache license v2](http://www.apache.org/licenses/LICENSE-2.0.html)

<h3>PackJacket</h3>
The independent [PackJacket](http://packjacket.sf.net/) opensource project offers a convenient graphical user interface for creating IzPack-based installers.

PackJacket is not affiliated with the IzPack project, and is released under the terms of the [GPLv3 license](http://www.gnu.org/licenses/gpl.html)

## Native launchers

We developed a simple Windows native launcher that can check for the presence of a Java Runtime, and install it if need be:

* [Version 2.2, based on Qt](http://dist.codehaus.org/izpack/native-launcher/izpack-launcher-2.2.zip)
* [Version 1.3, based on wxWidgets](http://dist.codehaus.org/izpack/native-launcher/izpack-launcher-1.3.zip)

You may alternatively look at the independent [JSmooth](http://jsmooth.sourceforge.net/) and [Launch4J](http://launch4j.sourceforge.net/) opensource projects. Lots of users have had positive experiences mixing them with IzPack based installers!

## Showcases

We have a few showcase that we designed in the past:

* [Installer for GlassFish v2.1.1 b31g](http://dist.codehaus.org/izpack/showcases/glassfish-install-v2.1.1-b31g.jar)
* [Installer for GlassFish v3 Prelude](http://dist.codehaus.org/izpack/showcases/glassfish-v3-prelude-install.jar)

The source code for building those installers is [available from our old Subversion repository](http://svn.codehaus.org/izpack-svn/izpack-showcases/).
