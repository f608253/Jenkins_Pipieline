pipeline {
        agent any
        stages {
              stage ('Compile stage') {
                    steps {
                           withMaven(maven : 'apache-maven-3.5.3'){
                             sh 'mvn clean compile'
                             }
                        }
                  }

               stage ('Testing stage') {
                    steps {
                           withMaven(maven : 'apache-maven-3.5.3'){
                             sh 'mvn test'
                             }
                        }
                  }

               stage ('Deployment stage') {
                    steps {
                           withMaven(maven : 'apache-maven-3.5.3'){
                             sh 'mvn deploy'
                             }
                        }
                  }
        }
}
