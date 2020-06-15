# MAVEN---Resource-Sharing-across-Projects
This project helps to share resource files through Maven across projects using Assembly and Dependency plugins.

## Apache Maven Assembly Plugin

The Assembly Plugin for Maven enables developers to combine project output into a single distributable archive that also contains dependencies, modules, site documentation, and other files.

Your project can easily build distribution "assemblies" using one of the prefabricated assembly descriptors. These descriptors handle many common operations, such as packaging a project's artifact along with generated documentation into a single zip archive. Alternatively, your project can provide its own descriptor and assume a much higher level of control over how dependencies, modules, file-sets, and individual files are packaged in the assembly.

Currently it can create distributions in the following formats:
1. zip
2. tar
3. tar.gz (or tgz)
4. tar.bz2 (or tbz2)
5. tar.snappy
6. tar.xz (or txz)
7. jar
8. dir
9. war
10. and any other format that the ArchiveManager has been configured for

STEPS OF EXECUTION
------------------
Step 1. Resource Sharing: contains the files to be shared accross the maven projects. On running command: mvn clean install -> this will create a zip file containing all the files in resources

Step 2. Resource User: on running "mvn clean install" will unzip the file in the target/generated-resources directory.

Step 3. Then, resource files can be used as per the usage in the project.

