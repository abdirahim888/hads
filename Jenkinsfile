pipeline {
    agent any

    environment {
        SONAR_SCANNER_HOME = 'C:\\sonar-scanner-5.0.1.3006-windows\\bin'
        SONAR_HOST_URL = 'http://localhost:9000'
        SONAR_PROJECT_KEY = 'TESTING YOUR CURRENCY CONVERSION APP'
        SONAR_LOGIN = 'sqp_18f0517dfb2cd286f0f28920478212878a9dd807'
    }

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/abdirahim888/hads.git'
            }
        }

        stage('abdirahim2') {
            steps {
                withSonarQubeEnv('abdirahim2') {
 bat "C:\\sonar-scanner-5.0.1.3006-windows\\bin\\sonar-scanner -Dsonar.projectKey=TESTING YOUR CURRENCY CONVERSION APP -Dsonar.sources=task9\\src/main/java -Dsonar.host.url=http://localhost:9000 -Dsonar.login=sqp_18f0517dfb2cd286f0f28920478212878a9dd807"               
              }
            }
        }
    }
}
