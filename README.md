       apt update
       INSTALL JAVA & MAVEN
       ====================
       #apt-get update 
       #apt-get install java 
       #apt-get install tomcat9 -y 
       #apt-get install maven -y  
       #mvn -version 
       
       Distribution Installation
       ===========================
       
       #vi ~/.profile open this file and give path insert below content
       
       export JAVA_HOME="/opt/jdk1.8.0_151" 
       export PATH=$JAVA_HOME/bin:$PATH 
       export CATALINA_HOME="/opt/apache-tomcat-9.0.2" 
       export PATH=$CATALINA_HOME/bin:$PATH 
       export M2_HOME="/opt/apache-maven-3.5.2" 
       export PATH=$M2_HOME/bin:$PATH 
        
        
        export CATALINA_HOME="/opt/apache-tomcat-9.0.2" 
       export PATH=$CATALINA_HOME/bin:$PATH
       
       CLONE FROM GITHUB
       =================
       
        #git clone https://github.com/Gopikrishna242/users.git
        
        #cd /user
        
        #mvn build
        #mvn clean
        #mvn clean install
        #mvn package
        
        the build was sucessfull
       
    INSTALL Tomcat9
    ===============
    apt install tomcat9
    vi /var/lib/tomcat9/conf/tomcat-users.xml
  
    edit and add user and passwrd , and manager-GUI,user-GUI,
    
    <user username="admin" password="admin" roles="manager-gui,admin-gui,admin-script"/>
     
     to start service
    ================
    
    systemctl restart tomcat9.service
    systemctl status tomcat9.service
    
    take IP-adress of server and place connect with port number 8080
    ================================================================
    
    http://18.232.136.52:8080
    
    open manager app and give username and password login for tomcat-server
   
    apt install tomcat9-docs
    apt install tomcat9-examples
    apt install tomcat9-admin
    
    copy JAR file to Tomcat default location
  
    cp users-api-0.0.1.jar /var/lib/tomcat9/webapps/
  
  
  
