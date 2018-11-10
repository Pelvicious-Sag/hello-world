node {
    checkout scm

    def customImage = docker.build(ruby:2.5)

    customImage.inside {
        sh 'hello_world.rb'
    }
}
