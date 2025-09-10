<?xml version="1.0" encoding="UTF-8"?>

<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
  <modelVersion>4.0.0</modelVersion>
  <groupId>SE</groupId>
  <artifactId>CMS</artifactId>
  <version>0.0.1-SNAPSHOT</version>
  <packaging>war</packaging>

  <name>CMS Maven Webapp</name>
  <!-- FIXME change it to the project's website -->
  <url>http://www.example.com</url>

  <properties>
    <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
    <maven.compiler.source>8</maven.compiler.source>
    <maven.compiler.target>8</maven.compiler.target>
  </properties>
  <dependencies>
    <dependency>
      <groupId>junit</groupId>
      <artifactId>junit</artifactId>
      <version>4.13.1</version>
      <scope>test</scope>
    </dependency>
  </dependencies>
  
  <dependencyManagement>
    <dependencies>
        <dependency>
            <groupId>group.id</groupId>
            <artifactId>artifact-id</artifactId>
            <version>desired-version</version>
        </dependency>
        <dependency>
    		<groupId>some.group</groupId>
    		<artifactId>some-artifact</artifactId>
    		<version>1.0</version>
    	<exclusions>
        	<exclusion>
            	<groupId>conflicting.group</groupId>
            	<artifactId>conflicting-artifact</artifactId>
        	</exclusion>
    	</exclusions>
		</dependency>
		<dependency>
    		<groupId>jsp</groupId>
    		<artifactId>jsp</artifactId>
    		<version>2.0.0</version>
		</dependency>
		<dependency>
    		<groupId>web</groupId>
    		<artifactId>jsp</artifactId>
    		<version>2.0.0</version>
		</dependency>
		<dependency>
    		<groupId>ja</groupId>
    		<artifactId>jstl</artifactId>
    		<version>1.2</version>
		</dependency>
    </dependencies>
</dependencyManagement>


  <build>
    <finalName>CMS</finalName>
    <pluginManagement>
      <plugins>
        <plugin>
          <artifactId>maven-antrun-plugin</artifactId>
          <version>3.1.0</version>
        </plugin>
        <plugin>
          <artifactId>maven-assembly-plugin</artifactId>
          <version>3.6.0</version>
        </plugin>
        <plugin>
          <artifactId>maven-dependency-plugin</artifactId>
          <version>3.6.1</version>
        </plugin>
        <plugin>
          <artifactId>maven-release-plugin</artifactId>
          <version>3.0.1</version>
        </plugin>
        <plugin>
          <artifactId>maven-clean-plugin</artifactId>
          <version>3.4.0</version>
        </plugin>
        <plugin>
          <artifactId>maven-resources-plugin</artifactId>
          <version>3.3.1</version>
        </plugin>
        <plugin>
          <artifactId>maven-compiler-plugin</artifactId>
          <version>3.13.0</version>
        </plugin>
        <plugin>
          <artifactId>maven-surefire-plugin</artifactId>
          <version>3.3.0</version>
        </plugin>
        <plugin>
          <artifactId>maven-war-plugin</artifactId>
          <version>3.4.0</version>
        </plugin>
        <plugin>
          <artifactId>maven-install-plugin</artifactId>
          <version>3.1.2</version>
        </plugin>
        <plugin>
          <artifactId>maven-deploy-plugin</artifactId>
          <version>3.1.2</version>
        </plugin>
      </plugins>
    </pluginManagement>
  </build>
  
</project>
