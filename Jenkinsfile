node {
    checkout scm

    def customImage = docker.build('ruby')

    customImage.inside {
        sh 'ruby hello_world.rb'
    }
}
