To facilitate OSGi bundle manifest generation, the archetype offers the choice of two maven plugins.

a. SpringSource Bundlor Plugin 
Home page: http://www.springsource.org/bundlor

"SpringSource® Bundlor is a tool that automates the detection of dependencies and the creation of OSGi 
manifest directives for JARs after their creation."

The Bundlor tool is enabled by default.

b. Apache Felix Bundle Plugin
Home page: http://felix.apache.org/site/apache-felix-maven-bundle-plugin-bnd.html

"This plugin for Maven 2 is based on the BND tool from Peter Kriens. [...] The way you create a bundle 
with BND is to tell it the content of the bundle's JAR file as a subset of the available classes."


To trigger the manifest generation (using either plugin), run: mvn package

<?xml version="1.0" encoding="UTF-8"?>
<classpath>
	<classpathentry kind="src" path="src/main/java"/>
	<classpathentry kind="src" path="src/main/resources"/>
	<classpathentry kind="src" output="target/test-classes" path="src/test/java"/>
	<classpathentry kind="src" output="target/test-classes" path="src/test/resources"/>
	<classpathentry kind="con" path="org.eclipse.jdt.launching.JRE_CONTAINER"/>
	<classpathentry kind="con" path="org.eclipse.pde.core.requiredPlugins"/>
	<classpathentry kind="var" path="M2_REPO/org/junit/com.springsource.junit/3.8.2/com.springsource.junit-3.8.2.jar"/>
	<classpathentry kind="var" path="M2_REPO/org/springframework/org.springframework.test/2.5.6.SEC01/org.springframework.test-2.5.6.SEC01.jar"/>
	<classpathentry kind="var" path="M2_REPO/org/springframework/org.springframework.core/2.5.6.SEC01/org.springframework.core-2.5.6.SEC01.jar"/>
	<classpathentry kind="var" path="M2_REPO/org/springframework/org.springframework.context/2.5.6.SEC01/org.springframework.context-2.5.6.SEC01.jar"/>
	<classpathentry kind="var" path="M2_REPO/org/springframework/org.springframework.beans/2.5.6.SEC01/org.springframework.beans-2.5.6.SEC01.jar"/>
	<classpathentry kind="var" path="M2_REPO/org/slf4j/com.springsource.slf4j.api/1.5.0/com.springsource.slf4j.api-1.5.0.jar"/>
	<classpathentry kind="var" path="M2_REPO/org/slf4j/com.springsource.slf4j.org.apache.commons.logging/1.5.0/com.springsource.slf4j.org.apache.commons.logging-1.5.0.jar"/>
	<classpathentry kind="var" path="M2_REPO/org/slf4j/com.springsource.slf4j.log4j/1.5.0/com.springsource.slf4j.log4j-1.5.0.jar"/>
	<classpathentry kind="var" path="M2_REPO/org/springframework/osgi/log4j.osgi/1.2.15-SNAPSHOT/log4j.osgi-1.2.15-SNAPSHOT.jar"/>
	<classpathentry kind="var" path="M2_REPO/org/eclipse/osgi/org.eclipse.osgi/3.2.2/org.eclipse.osgi-3.2.2.jar"/>
	<classpathentry kind="var" path="M2_REPO/org/springframework/osgi/spring-osgi-test/1.2.1/spring-osgi-test-1.2.1.jar"/>
	<classpathentry kind="var" path="M2_REPO/org/springframework/osgi/spring-osgi-mock/1.2.1/spring-osgi-mock-1.2.1.jar"/>
	<classpathentry kind="var" path="M2_REPO/org/springframework/osgi/spring-osgi-core/1.2.1/spring-osgi-core-1.2.1.jar"/>
	<classpathentry kind="var" path="M2_REPO/org/springframework/osgi/spring-osgi-extender/1.2.1/spring-osgi-extender-1.2.1.jar"/>
	<classpathentry kind="var" path="M2_REPO/org/springframework/osgi/spring-osgi-io/1.2.1/spring-osgi-io-1.2.1.jar"/>
	<classpathentry kind="var" path="M2_REPO/org/objectweb/asm/com.springsource.org.objectweb.asm/2.2.3/com.springsource.org.objectweb.asm-2.2.3.jar"/>
	<classpathentry kind="output" path="target/classes"/>
</classpath>

