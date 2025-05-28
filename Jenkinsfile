pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'maven_3_5_0') {
                    bat 'mvn clean compile'
                    bat 'echo Simulating compilation step...'

                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(maven : 'maven_3_5_0') {
                    bat 'mvn test'
                    bat 'echo Simulating testing step...'

                }
            }
        }


        // stage ('Deployment Stage') {
        //     steps {
        //         withMaven(maven : 'maven_3_5_0') {
        //             bat 'echo Simulating deployment step...'
        //             bat 'mvn deploy'
        //         }
        //     }
        // }
    }
}
