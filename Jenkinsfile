@Library('test_lib') _
pipeline{
    agent any
    stages{
        stage("Test"){
            steps{
                echo "========Testing========"
            }
            
        }
        stage("Build"){
            steps{
                   script{
                       buildJar()
                   }
            }
            
        }
        stage("Deploy"){
            when{
                expression{
                    BRANCH_NAME == "mein"
                }
            }
            steps{
                echo "========Deploy========"
            }
            
        }
    }
}
