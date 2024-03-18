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
                echo "========Building========"
            }
            
        }
        stage("Deploy"){
            when{
                expression{
                    BRANCH_NAME == "main"
                }
            }
            steps{
                echo "========Deploy========"
            }
            
        }
    }
}
