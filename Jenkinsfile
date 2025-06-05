pipeline {
    agent any

    stages {
        stage('Топ') {
            steps {
                script {
                    echo 'Состояние жестких дисков системы:'
                    sh 'df -h'
                }
            }
        }

        stage('Disk Usage Info') {
            steps {
                script {
                    echo 'Процесс, занимающий наибольший объем памяти системы, в текущий момент:'
                    sh 'ps -eo pid,comm,%mem --sort=-%mem | head -n 2'
                }
            }
        }
    }
}