pipeline{
    agent any
    stages{
        stage("Build"){
            steps{
                // git branch: 'main', changelog: false, credentialsId: 'github', poll: false, url: 'https://github.com/octobit8-pvt-ltd/django_app_PrathamBaliyan.git'
                bat 'python django_app.py'
            }


        }
    }
    post {
        always {
            mail (
                     subject: 'Jenkins Build Notification',
                     body: 'Successfully built post build in jenkins',
                     to: 'prathambaliyan012@gmail.com ,pratham.baliyan@octobit8.com'
                )

}

}

}