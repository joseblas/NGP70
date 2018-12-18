
pipeline {
    agent any
    options {
        checkoutExtensions( ["CleanCheckout"] )
    }
    stages {
        stage("foo") {
            steps {
                echo "hello"
                    script {
                        if (!fileExists("Jenkinsfile")) {
                            error "Jenkinsfile does not exist"
                        }
                    }
            }
        }
    }
}

