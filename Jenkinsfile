pipeline {
        agent any
        stages {
              stage ('Compile stage') {
                    steps {
                           withmaven(maven : 'apache-maven-3.5.3'){
                             sh 'mvn clean compile'
                             }
                        }
                  }

               stage Testing stage') {
                    steps {
                           withmaven(maven : 'apache-maven-3.5.3'){
                             sh 'mvn test'
                             }
                        }
                  }

               stage ('Deployment stage') {
                    steps {
                           withmaven(maven : 'apache-maven-3.5.3'){
                             sh 'mvn deploy'
                             }
                        }
                  }
