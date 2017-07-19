# simpleMavenExampleForPmdIntegration
Lets the build fail if there is a PMD violation


```                                                                     
------------------------------------------------------------------------
Building mavenproject1 1.0-SNAPSHOT
------------------------------------------------------------------------

--- maven-clean-plugin:2.4.1:clean (default-clean) @ mavenproject1 ---
Deleting /Users/markiewb/NetBeansProjects/mavenproject1/target

--- maven-resources-plugin:2.5:resources (default-resources) @ mavenproject1 ---
[debug] execute contextualize
Using 'UTF-8' encoding to copy filtered resources.
skip non existing resourceDirectory /Users/markiewb/NetBeansProjects/mavenproject1/src/main/resources

--- maven-compiler-plugin:2.3.2:compile (default-compile) @ mavenproject1 ---
Compiling 1 source file to /Users/markiewb/NetBeansProjects/mavenproject1/target/classes

--- maven-resources-plugin:2.5:testResources (default-testResources) @ mavenproject1 ---
[debug] execute contextualize
Using 'UTF-8' encoding to copy filtered resources.
skip non existing resourceDirectory /Users/markiewb/NetBeansProjects/mavenproject1/src/test/resources

--- maven-compiler-plugin:2.3.2:testCompile (default-testCompile) @ mavenproject1 ---
No sources to compile

--- maven-surefire-plugin:2.10:test (default-test) @ mavenproject1 ---
No tests to run.
Surefire report directory: /Users/markiewb/NetBeansProjects/mavenproject1/target/surefire-reports

-------------------------------------------------------
 T E S T S
-------------------------------------------------------

Results :

Tests run: 0, Failures: 0, Errors: 0, Skipped: 0


--- maven-jar-plugin:2.3.2:jar (default-jar) @ mavenproject1 ---
Building jar: /Users/markiewb/NetBeansProjects/mavenproject1/target/mavenproject1-1.0-SNAPSHOT.jar

>>> maven-pmd-plugin:3.8:check (check pmd and fail) @ mavenproject1 >>>

--- maven-pmd-plugin:3.8:pmd (pmd) @ mavenproject1 ---
Unable to locate Source XRef to link to - DISABLED

<<< maven-pmd-plugin:3.8:check (check pmd and fail) @ mavenproject1 <<<

--- maven-pmd-plugin:3.8:check (check pmd and fail) @ mavenproject1 ---
------------------------------------------------------------------------
BUILD FAILURE
------------------------------------------------------------------------
Total time: 3.560s
Finished at: Wed Jul 19 22:45:56 CEST 2017
Final Memory: 26M/312M
------------------------------------------------------------------------
Failed to execute goal org.apache.maven.plugins:maven-pmd-plugin:3.8:check (check pmd and fail) on project mavenproject1: 
You have 1 PMD violation. For more details see: /Users/markiewb/NetBeansProjects/mavenproject1/target/pmd.xml -> [Help 1]

To see the full stack trace of the errors, re-run Maven with the -e switch.
Re-run Maven using the -X switch to enable full debug logging.

For more information about the errors and possible solutions, please read the following articles:
[Help 1] http://cwiki.apache.org/confluence/display/MAVEN/MojoFailureException
```
