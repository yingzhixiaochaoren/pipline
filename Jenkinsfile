pipeline {
    agent any
    options {
        disableConcurrentBuilds() // 禁止并发构建
        timeout(time: 1, unit: 'HOURS') // 设置构建超时时间为1小时
        buildDiscarder(logRotator(numToKeepStr: '10')) // 保留最近的 10 次构建
    }
    stages {
        stage('Build') {
            steps {
                echo 'hello world form git'
            }
        }
    }
}
