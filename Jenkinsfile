@Library('pipeline-library-demo')_

pipeline {
    agent any
    stages {
        stage('Demo') {
            echo 'Hello World'
            sayHello 'Dave'
            }       
        
        stage('Example') {
            steps {
                echo "running on ${env.JENKINS_URL} for build number ${env.BUILD_ID} nd Job name ${env.JOB_NAME}" 
            }
        }
//defining environment variable and we can print all environment variables with printenv        
        stage('Example1') {
            environment { 
                DEBUG_FLAGS = '-g'
            }
            steps {
                sh 'printenv'
            }
        }

    }
}
