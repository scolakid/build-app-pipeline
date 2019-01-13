pipeline{
    agent any
    options {
        // Only keep the 10 most recent builds
        buildDiscarder(logRotator(numToKeepStr:'10'))
    }
    
    stages {
        stage ('Checkout'){
            steps{
                git branch: 'exampleBranch', url: 'https://github.com/example-org/example-repo.git'
            }
        }
        stage("foo"){
            steps {
                echo "hello"
            }
        }
    }
}