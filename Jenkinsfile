pipeline {
    agent any
     stages {
             stage('Kubernetes redis deployment') {
 steps {
                input 'Deploy to Production?'
                milestone(1)
                kubernetesDeploy(
                    kubeconfigId: 'kubeconfig',
                    configs: 'train-schedule-kube.yml',
                    enableConfigSubstitution: true
                )
                }
                }
                }
                }
