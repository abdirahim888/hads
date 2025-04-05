pipeline {
    agent any

    environment {
        SONAR_SCANNER_HOME = 'C:\\sonar-scanner-5.0.1.3006-windows\\bin'
        SONAR_HOST_URL = 'http://localhost:9000'
        SONAR_PROJECT_KEY = 'abdirahim1'
        SONAR_LOGIN = 'sqa_e22957c4542fd762a603156438da08c9422b574c'
    }

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/abdirahim888/hads.git'
            }
        }

        stage('abdirahim1') {
            steps {
                withSonarQubeEnv('SonarQube-Server') {
 bat "C:\\sonar-scanner-5.0.1.3006-windows\\bin\\sonar-scanner -Dsonar.projectKey=abdirahim1 -Dsonar.sources=src\\main\\java -Dsonar.host.url=http://localhost:9000 -Dsonar.login=sqa_e22957c4542fd762a603156438da08c9422b574c"                }
            }
        }
    }
}
