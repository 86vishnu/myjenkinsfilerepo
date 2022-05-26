pipeline {

agent any
stages {

     stage('SCM') {
            steps {
                git'https://github.com/86vishnu/simple-java-maven-app.git'
            }
}
     stage('Deploy') {
            steps {
               sh 'mvn clean package'
            }
}  
       
     stage('Test') {
           steps {
               sh 'java -jar target/*jar'
           }
}

 
}
}
