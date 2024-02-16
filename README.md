# Java-App-v3
========================<br/>
<h1>BUILD OUTPUT DESCRIPTION</h1><br/>
======================== <br/>
<br/><br/>
When you build a Java application project that has a main class, the IDE
automatically copies all of the JAR
files on the project's classpath to your projects dist/lib folder. The IDE
also adds each of the JAR files to the Class-Path element in the application
JAR files manifest file (MANIFEST.MF).
<br/><br/>
To run the project from the command line, go to the dist folder and
type the following:
<br/><br/>
|<code>java -jar "try.jar"</code>| --version 3(added title)|
<br/><br/>
To distribute this project, zip up the dist folder (including the lib folder)
and distribute the ZIP file.
<br/><br/>
Notes:
<br/><br/>
* If two JAR files on the project classpath have the same name, only the first
JAR file is copied to the lib folder.
* Only JAR files are copied to the lib folder.
If the classpath contains other types of files or folders, these files (folders)
are not copied.
* If a library on the project classpath also has a Class-Path element
specified in the manifest, the content of the Class-Path element has to be on
the project's runtime path.
* To set a main class in a standard Java project, right-click the project node
in the Projects window and choose Properties. Then click Run and enter the
class name in the Main Class field. Alternatively, you can manually type the
class name in the manifest Main-Class element.
<br/>
