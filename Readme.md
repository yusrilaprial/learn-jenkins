# Learn Jenkins

Learn Automation Server with Jenkins

## Software Requirements

- SSH
- Java
- Git
- Web Brower

## Setup

- Install Git on Server: `apt-get install git`
- Install Java on Server: `apt install openjdk-17-jdk-headless`
- Install Jenkins on Server:
  1. go to: https://www.jenkins.io/download/
  2. copy .war link: https://get.jenkins.io/war-stable/2.492.1/jenkins.war
  3. run: `wget https://get.jenkins.io/war-stable/2.492.1/jenkins.war`
  4. run: `java -jar jenkins.war --httpPort=9090 &`
  5. access app in port 9090
