pipeline {
    agent any
    
    stages {
        stage('Create User and Group') {
            steps {
                script {
                    sh '''
                        # Create a group
                        sudo groupadd mygroup
                        
                        # Create a user
                        sudo useradd -m myuser
                        
                        # Add the user to the group
                        sudo usermod -a -G mygroup myuser
                    '''
                }
            }
        }
    }
}
