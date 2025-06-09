CSSBox
======

[![Maven Central](https://maven-badges.herokuapp.com/maven-central/net.sf.cssbox/cssbox/badge.png)](https://maven-badges.herokuapp.com/maven-central/net.sf.cssbox/cssbox)

An HTML/CSS rendering engine library
(c) 2005-2024 Radek Burget (burgetr@fit.vutbr.cz)

See the project page for more information and downloads:
[http://cssbox.sourceforge.net/](http://cssbox.sourceforge.net/)

All the source code of the CSSBox itself is licensed under the GNU Lesser General
Public License (LGPL), version 3. A copy of the LGPL can be found 
in the LICENSE file.

CSSBox relies on the jStyleParser open source CSS parser 
[http://cssbox.sourceforge.net/jstyleparser](http://cssbox.sourceforge.net/jstyleparser).

The CSSBox library is under development and its API or functionality may change in future versions.
See the CHANGELOG for the most important changes to the previous versions.

Gradle and Jitpack support
--------------------------

This project now supports Gradle and Jitpack. After making a change, create a new release using the x.x.x format
(See: https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository)

If using in conjunction with CSSBox, you will then also need to update CSSBox's build.gradle.kts file and increment the version of jStyleParser
with the new version number.

Test Suite files
--------------------------

The CSSBox unit tests require many files to run correctly, all of which can be found at https://github.com/radkovo/CSSBoxTesting/

Due to how many test files there are, importing them manually and attempting to build can crash some IDEs like Eclipse. in these cases bulding via a CLI is needed.

These tests are imported and run using Github Actions, and so are not needed in this repository. To run these tests locally, create a directory called "testsuite" in the root,
and place the "baseline" folder from the CSSBoxTesting repo inside. Your directory should look like this:
```
CSSBox/testsuite/baseline/nightly-unstable/html4/...
```
When the test files files are absent the tests will not run locally.

