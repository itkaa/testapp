TestApp requires Java 5.

TOMCAT_HOME is your top level tomcat directory

## BUILDING AND RUNNING THE APPLICATION ##
run ant in this directory
copy dist/TestApp.war to ${TOMCAT_HOME}/webapps
NOTE: if you do not deploy via the .war you will additionally need to copy context.xml to ${TOMCAT_HOME}/conf/Catalina/localhost/TestApp.xml
start tomcat
browse to http://localhost:8080/TestApp
login with admin/admin, eddie/eddie, gary/gary or another profile defined in create_db.sql


## REDEPLOYING ##
stop tomcat ()
delete ${TOMCAT_HOME}/webapps/TestApp (delete the whole directory)
delete ${TOMCAT_HOME}/webapps/TestApp.war
follow the "building and runnig the application" instructions to deploy a fresh copy

## STARTING TOMCAT ##
run ${TOMCAT_HOME}/bin/startup

## STOPPING TOMCAT ##
run ${TOMCAT_HOME}/bin/shutdown

# All Rights Due to Contributors for Dependencey libraries hold


