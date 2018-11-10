node {
    def app

    stage('Clone repository') {
        
        checkout scm
    }

    stage('Build image') {

        app = docker.image('ruby')
    }

    stage('Test image') {

        app.inside {
            sh 'ruby hello_world.rb'
        }
    }
}
