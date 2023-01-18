pipeline {
    agent any
    options {
        buildDiscarder(logRotator(numToKeepStr: '3'))
        disableConcurrentBuilds()
    }
    parameters {
        string(
            name: 'pipelinejob',
            defaultValue: 'testjob',
            description: 'please provide the parameter'
        )
        choice(
            choices: [ '1', '2', '3', '4'],
            description: 'want to build this job',
            name: 'choicejob'
        )
    }
    stages {
        stage(start) {
            steps {
                echo 'this is my starting'
            }
        }
        stage('stage-A') {
            steps {
                echo  "this is my stage-A"
            }
        }
        stage('stage-B') {
            steps {
                echo "this is my stage-B"
            }
        }
        stage('stage-C') {
            steps {
                echo "this is my stage-C"
            }
        }
        stage('stage-D') {
            steps {
                echo " this is my stage-D"
            }
        }
    }
}
