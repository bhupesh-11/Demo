pipeline {
    agent any
    environment {
        name = 'Bhupesh'
    }
    parameters {
     string(name: 'Ananya',defaultValue: 'Patil', description: 'who are you ?')
    }
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Env') {
            input {
                message "Are you sure"
                ok "Yes Continue"
            }
            steps {
                bat  'echo %ananya%'
            }
        }
         stage('Prod') {
            environment {
        username = 'Prod'
    }
            steps {
                bat  'echo %username%'
            }
        }
    }
}
