# Learn Jenkins

Learn Automation Server with Jenkins

## Software Requirements

- SSH
- Java
- Git
- Web Browser

## Setup

- Install Git on Server: `apt-get install git`
- Install Java on Server: `apt install openjdk-21-jdk`
- Install Jenkins on Server:
  1. go to: https://www.jenkins.io/download/
  2. copy .war link: https://get.jenkins.io/war-stable/2.504.3/jenkins.war
  3. run: `wget https://get.jenkins.io/war-stable/2.504.3/jenkins.war`
  4. run Jenkins:
      - run in foreground: `java -jar jenkins.war --httpPort=9090`
      - run in background: `nohup java -jar jenkins.war > output.log 2>&1 --httpPort=9090 &`
  5. access app in port 9090
