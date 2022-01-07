pipeline {
    agent any

    stages {
        stage('contineous download blaster') {
            steps {
               git 'https://github.com/Chandudhfp/DemoATC.git'
            }
        }
         stage('contineous build') {
            steps {
               sh 'mvn install'
            }
        }
        stage('contineous deploy') {
            steps {
               sh 'cp target/DemoATR.war /opt/apache-tomcat-9.0.56/webapps'
            }
        }
        
    }
}
