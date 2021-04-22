## This repository is a fork from - https://github.com/keycloak/keycloak-quickstarts;

We did some changes to make it easier to run **service-jee-jaxrs** and **app-jee-html5** applications on **Openshift** without needing to spend much time configuring Keycloak adapter on Wildfly / JBoss application server;

**YOU CAN USE THIS REPOSITORY TO DEPLOY KEYCLOAK APPLICATIONS ON OPENSHIFT IN ORDER TO MAKE SOME DEMONSTRATIONS AND SEE HOW THE PRODUCT CAN PROTECT YOU APPLICATIONS**

# <span>Keycloak</span> Quickstarts

<span>Keycloak</span> is an Open Source Identity and Access Management solution for modern Applications and Services.

The quickstarts demonstrate securing TWO applications with <span>Keycloak</span>. 

Below you can see the topology of this project and check how we protect those applications using keycloak;

![](docs/keycloak-demo.png)


0. [Deploying service-jee-jaxrs application on Openshift](#testdrive-step-0)


### Deploying service-jee-jaxrs application on Openshift <a name="testdrive-step-0"></a>

The **service-jee-jaxrs** application runs on top of Red Hat JBoss EAP Server 7.0 or Wilfdly 10. The service-jee-jaxrs application requires the keycloak adapter installed into the JBoss or Widlfly Server as described here: https://github.com/keycloak/keycloak-quickstarts/blob/latest/docs/getting-started.md#wildfly.

Inside the **sso-eap7-bin-demo/configuration/** directory we have the **standalone-openshift.xml** file that is basically the standalone.xml file with the keycloak adapter module configuration (I've added the module into my JBoss Application Server running locally).

The **sso-eap7-bin-demo/modules/** directory we have the modules that will be loaded by our JBoss / Wildfly Application Server runing on Openshift later;






