pipeline {
    agent any

    environment {
        SONAR_SCANNER_HOME = 'C:\\sonar-scanner-5.0.1.3006-windows\\bin'
        SONAR_HOST_URL = 'http://localhost:9000'
        SONAR_PROJECT_KEY = 'task9'
        SONAR_LOGIN = 'sqp_80cec4c69e4d3c1522bec68bf8777bb429e4abdc'
    }

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/abdirahim888/hads.git'
            }
        }

        stage('abdirahim4') {
            steps {
                withSonarQubeEnv('abdirahim4') {
 bat "C:\\sonar-scanner-5.0.1.3006-windows\\bin\\sonar-scanner -Dsonar.projectKey=task9 -Dsonar.sources=task9\\src/main/java -Dsonar.host.url=http://localhost:9000 -Dsonar.login=sqp_80cec4c69e4d3c1522bec68bf8777bb429e4abdc"               
              }
            }
        }
    }
}
