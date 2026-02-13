pipeline{

    agent any

    stages{

        stage("compile"){
            steps{
                bat 'javac Test.java'
            }
        }

        stage("run"){
            steps{
                bat 'java Test'
            }
        }
    }

    post{
         success{
             bat 'echo "Build Success"'
         }
         failure{
              bat 'echo "Build Failure"'
         }
    }
}
