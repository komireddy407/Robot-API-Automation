pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh '''Set Path=%PYTHON_HOME%;%Path%
Library/Lib.bat
rmdir /s /q output
rmdir output
robot --listener allure_robotframework AllCases
exit 0'''
      }
    }

  }
}