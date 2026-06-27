pipeline {
    agent any

    stages {
        stage('Use Secret') {
            steps {
                withCredentials([
                    usernamePassword(
                        credentialsId: 'passwd-slave-jenkins-',
                        usernameVariable: 'USERNAME',
                        passwordVariable: 'PASSWORD'
                    )
                ]) {
                    sh '''
                        echo "Username: $USERNAME"
                        if [ -n "$PASSWORD" ]; then
                            echo "Password is available"
                        fi
                    '''
                }
            }
        }
    }
}
