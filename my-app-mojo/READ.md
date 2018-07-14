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


