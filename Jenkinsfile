pipeline {
    agent any
     stages {
        stage ('Compile Stage') {

            steps {
                //withMaven(maven : 'maven_3_5_0') {
                    sh 'mvn clean compile'
              //  }
            }
        }
        stage('Build') {
            steps {
             //    withMaven(maven : 'maven_3_5_0') {
                    sh 'mvn  -B -DskipTests clean package'
                }
             // }
        }
        stage ('Testing Stage') {

            steps {
                withMaven(maven : 'maven_3_5_0') {
                    sh 'mvn test'
                }
            }
             post {
                always {
                    junit 'target/surefire-reports/*.xml'
                }
            }
        }
        
    }
}
