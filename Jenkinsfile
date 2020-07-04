node {
    
	

    env.AWS_ECR_LOGIN=true
    def newApp
    def registry = 'gustavoapolinario/microservices-node-todo-frontend'
    def registryCredential = 'dockerhub'
	
	stage('Git') {
		git 'https://github.com/gustavoapolinario/node-todo-frontend'
	}
	stage('Build') {
		sh 'npm install'
	}
	stage('Test') {
		sh 'npm test'
	}
stage('Build') {
        
            sh 'npm run build'
            echo "Build completed"
        
        
    }
	 stage('Package Build') {
        sh "tar -zcvf bundle.tar.gz dist/automationdemo/"
    }

 
    
}
