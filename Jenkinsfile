pipeline {
    agent any
    tools {
        maven "Maven3"
        jdk "OracleJDK8"
    }
    environment {
        SNAP_REPO = 'vprofile-snapshot'
        NEXUS_USER = 'admin'
        NEXUS_PASS = 'Munna@6344!'
        RELEASE_REPO = 'vrprofile-release'
        CENTRAL_REPO = 'vpro-maven-central'
        NEXUS_IP = '172.31.44.93'
        NEXUS_PORT = '8081'
        NEXUS_GRP_REPO = 'vpro-maven-group'
        NEXUS_LOGIN = 'nexuslogin'
    }
    stages {
        stage('Build'){
            steps {
                sh 'mvn -s settings.xml -DskipTests install'
            }
        }

    }
}