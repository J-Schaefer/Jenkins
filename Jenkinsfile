pipeline {
  agent { label "linux" }
  stages {
    stage("build") {
      steps {
        sh """
          docker build -t ros_noetic_Dockerfile .
        """
      }
    }
    stage("run") {
      steps {
        sh """
          docker run --rm ros_noetic_Dockerfile
        """
      }
    }
  }
}
