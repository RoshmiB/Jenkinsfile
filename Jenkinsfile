@Library('pipeline-library-demo')_

pipeline {
    agent none
       stage ('Example') {
        steps {
             script { 
                 echo 'Hello World'
                 sayHello 'Dave'
             }
        }
    }
}
