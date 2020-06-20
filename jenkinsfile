pipeline {
    agent any
     stages {
             stage('Kubernetes redis deployment') {
 steps {
                input 'Deploy to Production?'
                milestone(1)
                kubernetesDeploy(
                    kubeconfigId: 'kubeconfig',
                    configs: 'redis.yaml',
                    enableConfigSubstitution: true
                )
                }
                }
                }
                }
