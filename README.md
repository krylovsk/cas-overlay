cas-overlay
==================

Forked from https://github.com/github/cas-overlay, this overlay configures Jasig CAS v4.1.0-SNAPSHOT for use with a [LDAP server](http://jasig.github.io/cas/development/installation/LDAP-Authentication.html) + [OAuth2])(http://jasig.github.io/cas/development/protocol/OAuth-Protocol.html) and [REST Protocols](http://jasig.github.io/cas/development/protocol/REST-Protocol.html). 

Currently, this overlay is configured for LDAP Direct Bind. For configuration against an authenticated search or AD search, please refer to https://jasig.github.io/cas/4.0.0/installation/LDAP-Authentication.html to configure an alternate configuration manager.

# Versions
```xml
<cas.version>4.1.0-SNAPSHOT</cas.version>
```

# Requirements
* Apache Maven 3
* Web Server (i.e. Apache Tomcat 7)

# Configuration
All configuration is provided in src/man/webapp/WEB-INF. See [documentation](http://jasig.github.io/cas/development/installation/Maven-Overlay-Installation.html) for more info.

# Building
* Execute `mvn clean package`
* Copy the file over to `$CATALINA_HOME/conf/Catalina/localhost`
* Restart tomcat.
