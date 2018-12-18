## Security Testing Framework Overview
BDD-Security is a security testing framework that uses Behaviour Driven Development concepts to create self-verifying security specifications.

The framework is a set of Cucumber-JVM features that are pre-wired with [Selenium WebDriver](https://www.seleniumhq.org) and [OWASP ZAP](https://www.owasp.org/index.php/OWASP_Zed_Attack_Proxy_Project). (Some tests also utiltize [SSLyze](https://github.com/nabla-c0d3/sslyze) and [Tennable's Nessus scanner](http://www.tenable.com/products/nessus-vulnerability-scanner).)

It tests Web Applications and API's from an external point of view and does not require access to the target source code.

## Overview
**Requirements**
- JDK
- Gradle

**Directories**
- Security test features are defined in `src/test/resources/features`
- ZAP definitions are defined in `src/test/java/net/contiuumsecurity/steps`
- Selenium step definitions are defined in `src/test/java/net/contiuumsecurity/examples` 
- Test reports are placed in `build`

## Execution

 Launch the demo application

    $ java -jar ropeytasks.jar

Execute ZAP security test scenarios

    $ ./gradlew