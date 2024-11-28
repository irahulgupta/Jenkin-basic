Basic CICD Jenkin command for beginner

pipeline{
    agent any;
    stages{
        stage("Code"){
            steps{
               echo "Code wali stage" 
            }
        }
        stage("Build"){
            steps{
                echo "Build wali stage"
            }
        }
        stage("Test"){
            steps{
                echo "Test wali stage"
            }
        }
        stage("Deploy"){
            steps{
                sh "date"
            }
        }
    }
}
