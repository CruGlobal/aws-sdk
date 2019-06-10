# AWS SDK AEM project

This is a project is use to manage the AWS JAVA SDK files and dependencies.

## Modules
```
ion-java - 1.0.2
jackson-dataformat-cbor - 2.6.7
netty-codec-http - 4.1.17.Final
netty-transport - 4.1.17.Final
netty-resolver - 4.1.17.Final
netty-handler - 4.1.17.Final
netty-buffer - 4.1.17.Final
netty-codec - 4.1.17.Final
netty-common - 4.1.17.Final
aws-java-sdk-osgi - 1.11.534

```

## Update version

Under `ui.apps` edit pom.xml dependencies. 

## How to build

To build all the modules run in the project root directory the following command with Maven 3:

    mvn clean install

If you have a running AEM instance you can build and package the whole project and deploy into AEM with  

    mvn clean install -PautoInstallPackage

Or to deploy it to a publish instance, run

    mvn clean install -PautoInstallPackagePublish

Or alternatively

    mvn clean install -PautoInstallPackage -Daem.port=4503

Or to deploy only the bundle to the author, run

    mvn clean install -PautoInstallBundle
