pipeline {
    agent { 
        node {
            label 'agent-alpine-python3'
            }
      }
      
    triggers {
        pollSCM '*/1 * * * *'
    }

    stages {
        stage('Build') {
            steps {
                echo "Building.."
                sh '''
                echo "doing build stuff.."
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh '''
                echo "doing test stuff..
                '''
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                sh '''
                echo "doing delivery stuff.."
                '''
            }
        }
    }

    // stages {
    //     stage('Build') {
    //         steps {
    //             echo "Building.."
    //             sh '''
    //             cd myapp
    //             pip install -r requirements.txt
    //             '''
    //         }
    //     }
    //     stage('Test') {
    //         steps {
    //             echo "Testing.."
    //             sh '''
    //             cd myapp
    //             python3 hello.py
    //             python3 hello.py --name=Brad
    //             '''
    //         }
    //     }
    //     stage('Deliver') {
    //         steps {
    //             echo 'Deliver....'
    //             sh '''
    //             echo "doing delivery stuff.."
    //             '''
    //         }
    //     }
    // }
}