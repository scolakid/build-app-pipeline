pipeline{
    agent{label 'windows'}
        
    stages {
        stage("foo"){
            steps {
                echo "hello"
            }
        }
        stage("build"){
            steps{

		        bat "\"${tool 'MSBuild'}\" BuildApp.csproj /p:Configuration=Release /p:Platform=\"Any CPU\" /p:ProductVersion=1.0.0.${env.BUILD_NUMBER}"

            }
        }
    }
}