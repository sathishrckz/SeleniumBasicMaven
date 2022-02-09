pipeline{

agent any

    stages{

        stage ('Compile stage'){
            steps{
                 withMaven(maven : 'maven_3_8_4'){
                sh 'mvn clean compile'

                  }
            }
        }

        stage ('Testing stage'){
                    steps{
                         withMaven(maven : 'maven_3_8_4'){
                        sh 'mvn test'

                          }
                    }
        }
         stage ('Deployment stage'){
                            steps{
                                 withMaven(maven : 'maven_3_8_4'){
                                sh 'mvn deploy'

                                  }
                            }
         }


    }



}
