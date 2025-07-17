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
      - run in background: `nohup java -jar jenkins.war --httpPort=9090 > output.log 2>&1 &`
  5. access app in port 9090

## Build Steps

Build steps are the actions that Jenkins will perform to build your project. You can add multiple build steps, such as:
- Execute shell commands
- Invoke Ant or Maven targets
- Run Gradle tasks
- Send notifications
- Archive artifacts

## Build History

The build history shows the past builds of your project. You can view the status, duration, and console output of each build. You can also re-run previous builds or delete them if needed.

## Post Build Actions

Post build actions are the tasks that Jenkins will perform after the build is complete. These can include:
- Sending notifications (email, Slack, etc.)
- Archiving artifacts
- Triggering other builds
- Deploying to servers
- Running post-build scripts

## Copy Job

Copying a job in Jenkins allows you to create a new job based on an existing one. This is useful for creating similar jobs without starting from scratch.

## Build Periodically

You can schedule builds to run at specific intervals using cron syntax. This is useful for regular tasks like backups or updates.

## Poll SCM

You can configure Jenkins to poll your source code management (SCM) system for changes at regular intervals. If changes are detected, Jenkins will trigger a build automatically.

## Disable Job

You can disable a job in Jenkins to prevent it from running. This is useful when you want to pause a job without deleting it. Disabled jobs will not be triggered by builds or SCM changes.

## Jenkins Environment Variables

Jenkins provides a set of environment variables that can be used in your build steps.

## Global Environment Variables

You can define global environment variables in Jenkins that will be available to all jobs. This is useful for storing configuration values or secrets that need to be accessed by multiple jobs.

## Build Parameters

You can define parameters for your builds, allowing users to input values when triggering a build. This is useful for jobs that require user input or configuration.

## Discard Old Builds

You can configure Jenkins to automatically discard old builds to save disk space. You can set limits on the number of builds to keep or the age of builds to retain.

## Build Executors

Jenkins uses build executors to run jobs. Each executor can run one job at a time. You can configure the number of executors in the Jenkins system settings.

## Trigger Builds Remotely

You can trigger builds remotely using a URL with a specific token. This is useful for integrating Jenkins with other systems or triggering builds from scripts.

## View Group

You can view and manage groups of jobs in Jenkins. This allows you to organize jobs into categories for easier management.

## Nodes

You can configure nodes (also known as agents) in Jenkins to distribute builds across multiple machines. This allows for parallel execution and better resource utilization.
