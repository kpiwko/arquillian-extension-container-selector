Arquillian Container Selector Extension
=======================================

Allows alternative way of setting default container configuration in arquillian.xml:


    <container qualifier="openshift">
        <configuration>
        </configuration>
    </container>

    <container qualifier="openshift2">
        <configuration>
        </configuration>
    </container>

    <extension qualifier="container-selector">
        <property name="default">openshift1</property>
    </extension>

This allows you to set active container via Maven property filtering, thus in a much more friendly way for an IDE. This extension disables default ContainerExtension.
