##Report_2 trobleshooting

######Step1
![alt text](https://github.com/YauheniLikhachou/mntlab/blob/master/troubleshooting/sources/Screenshot.png)

######Step2
![alt text](https://github.com/YauheniLikhachou/mntlab/blob/master/troubleshooting/sources/Screenshot-1.png)

######Step3
![alt text](https://github.com/YauheniLikhachou/mntlab/blob/master/troubleshooting/sources/Screenshot-30.png)

######Step4
![alt text](https://github.com/YauheniLikhachou/mntlab/blob/master/troubleshooting/sources/Screenshot-40.png)

######Step5
![alt text](https://github.com/YauheniLikhachou/mntlab/blob/master/troubleshooting/sources/Screenshot-4.png)

######Step6
![alt text](https://github.com/YauheniLikhachou/mntlab/blob/master/troubleshooting/sources/Screenshot-5.png)

######Step7
![alt text](https://github.com/YauheniLikhachou/mntlab/blob/master/troubleshooting/sources/Screenshot-6.png)

######Step8
![alt text](https://github.com/YauheniLikhachou/mntlab/blob/master/troubleshooting/sources/Screenshot-7.png)

######Step9
![alt text](https://github.com/YauheniLikhachou/mntlab/blob/master/troubleshooting/sources/Screenshot-8.png)

######Step10
![alt text](https://github.com/YauheniLikhachou/mntlab/blob/master/troubleshooting/sources/Screenshot-9.png)
![alt text](https://github.com/YauheniLikhachou/mntlab/blob/master/troubleshooting/sources/Screenshot-10.png)

####Answers on the questions:
######1. What java version is installed?
          Run command "java -version" 
          java version "1.7.0_79" 
          Java(TM) SE Runtime Environment (build 1.7.0_79-b15) 
          Java HotSpot(TM) 64-Bit Server VM (build 24.79-b02, mixed mode) 
          
######2. How was it installed and configured?
           “/opt/oracle/java/x64//jdk1.7.0_79/bin/java” 
           # alternatives --config java
          
######3. Where are log files of tomcat and httpd?
          Logs of httpd: /var/log/httpd/  
          Logs of tomcat: /opt/apache/tomcat/7.0.62/logs/
          
######4. Where is JAVA_HOME and what is it?
          Path: opt/oracle/java/x64/jdk1.7.0_79
          JAVA_HOME is a variables of point to locate JDK and JRE to other applications.
          
######5. Where is tomcat installed?    
          TPath: /opt/apache/tomcat/7.0.62/
          
######6. What is CATALINA_HOME?
          CATALINA_HOME is a variable home tomcat directory.
          
######7. What users run httpd and tomcat processes? How is it configured?
          HTTPD service run apache user. Path: /etc/httpd/conf/httpd.conf
          TOMCAT service run tomcat user. Path: /etc/init.d/tomcat
          
######8. What configuration files are used to make components work with each other?
          /etc/httpd/conf/httpd.conf;
          /etc/httpd/conf.d/vhost.conf;
          /etc/httpd/conf.d/workers.properties;
          /opt/apache/tomcat/7.0.62/conf/server.xml.
          
######9. What does it mean: “load average: 1.18, 0.95, 0.83”?
          Load average is the average number of processes waiting for the CPU resources of the three time periods: 1.18 for 1 min, 0.95  for 5 min, 0.83 for 15 min
          
