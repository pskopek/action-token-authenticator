Source: <https://github.com/keycloak/keycloak-quickstarts>  


What is it?
-----------

This is example of how to setup dependency management in order to compile your extension using artifacts supplied in Red Hat GA maven repository. 
The code is untested and is present just to show compilation setup.

How to run the example?
-----------------------

Prerequisities:

1. maven version 3.9.z 

2. Java JDK 8

Run this command:

    mvn -s mvn-settings.xml clean install

Note: the mvn-settings.xml content. It uses empty local maven repository cache.
It uses just Red Hat GA maven repository together with maven central. 

keycloak-services artifact needs exclusions as set in [pom.xml lines 70-73](https://github.com/pskopek/action-token-authenticator/blob/5be50b3febb17be361d7c8ba1e6a5f7e844bae65/pom.xml#L70-L73).
