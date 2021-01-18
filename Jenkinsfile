pipeline {
   agent any
    stages {
      stage('SCM Checkout') {
         steps {
            git 'https://github.com/Santhosh1811/simple-java-maven-app'
        }
    }
    stage ('Build') {
        steps {
            sh '/opt/maven/bin/mvn clean verify -Dmaven.test.skip=true'
        }
    }
}
}
