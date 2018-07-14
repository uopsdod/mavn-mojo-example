how to build: 
mvn clean install

how to use this plugin: 
1. java doc-style mojo: 
mvn com.mycompany.app:my-app-mojo:1.0-SNAPSHOT:touch
2. java annotation-stlye mojo:
mvn com.mycompany.app:my-app-mojo:1.0-SNAPSHOT:touch2

expected result: 
1. you'll see a file named 'touch.txt' in the project root directory
2. you'll see s file named 'touch2.txt' in the project root directory

plugin prefix: 
STEP01 - add maven-plugin-plugin prefix setting to pom.xml 
STEP02 - add pluginGroup to maven-3.5.3/config/settings.xml:
  <pluginGroups>
	<pluginGroup>com.mycompany.app</pluginGroup>
  </pluginGroups>
STEP03 - test it: 
mvn fCustom:touch

bug after adding prefix setting: 
annotation-based plugin is broken(the commands below are not working):
mvn fCustom:touch2
mvn com.mycompany.app:my-app-mojo:1.0-SNAPSHOT:touch2





