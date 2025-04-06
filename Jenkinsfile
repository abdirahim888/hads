pipeline {
    agent any

    environment {
        SONAR_SCANNER_HOME = 'C:\\sonar-scanner-5.0.1.3006-windows\\bin'
        SONAR_HOST_URL = 'http://localhost:9000'
        SONAR_PROJECT_KEY = 'TESTING YOUR CURRENCY CONVERSION APP'
        SONAR_LOGIN = 'sqp_e6debce1845d007a0323f638c7a1618779924323'
    }

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/abdirahim888/gas.git'
            }
        }

        stage('abdirahim2') {
            steps {
                withSonarQubeEnv('abdirahim2') {
 bat "C:\\sonar-scanner-5.0.1.3006-windows\\bin\\sonar-scanner -Dsonar.projectKey=TESTING YOUR CURRENCY CONVERSION APP -Dsonar.sources=task9\\src/main/java -Dsonar.host.url=http://localhost:9000 -Dsonar.login=sqp_e6debce1845d007a0323f638c7a1618779924323"               
              }
            }
        }
    }
}
