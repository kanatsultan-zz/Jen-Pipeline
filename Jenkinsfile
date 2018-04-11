pipeline {
    agent any

    stages {
        stage ('Compile Stage2') {

            steps {
                withMaven(maven : 'maven_3_5_3') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage2') {

            steps {
                withMaven(maven : 'maven_3_5_3') {
                    sh 'mvn test'
                }
            }
        }


        stage ('Deployment Stage2') {
            steps {
                withMaven(maven : 'maven_3_5_3') {
                    sh 'mvn deploy'
                }
            }
        }
    }
}
