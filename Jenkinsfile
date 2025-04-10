pipeline {
    agent any

    environment {
        SONAR_SCANNER_HOME = 'C:\\sonar-scanner-5.0.1.3006-windows\\bin'
        SONAR_HOST_URL = 'http://localhost:9000'
        SONAR_PROJECT_KEY = 'task10'
        SONAR_LOGIN = 'sqp_350a6d2da80b6ae1be0a83de2ca15a89e36c8184'
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
 bat "C:\\sonar-scanner-5.0.1.3006-windows\\bin\\sonar-scanner -Dsonar.projectKey=task10 -Dsonar.sources=task9\\src/main/java -Dsonar.host.url=http://localhost:9000 -Dsonar.login=sqp_350a6d2da80b6ae1be0a83de2ca15a89e36c8184"               
              }
            }
        }
    }
}
