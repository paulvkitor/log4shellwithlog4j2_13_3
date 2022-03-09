# log4shellwithlog4j2_13_3
Springboot web application accepts a name get parameter and logs its value to log4j2.  Vulnerable to CVE-2021-44228.

# build the Springboot vulnerable application with
mvn clean install

# run the Springboot application with the k2 agent with
java --add-modules java.sql -javaagent:/opt/k2-ic/K2-JavaAgent-1.0.0-jar-with-dependencies.jar -jar target/demoLog4Shellwithlog4j2ver2_13_3-0.0.1-SNAPSHOT.jar
