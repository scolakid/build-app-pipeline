pipeline{
    agent any
    options {
        // Only keep the 10 most recent builds
        buildDiscarder(logRotator(numToKeepStr:'10'))
    }

    stages {
        stage("foo"){
            steps {
                echo "hello"
            }
        }
    }
}