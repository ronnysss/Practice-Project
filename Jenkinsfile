node(''){
stage('Initialise'){
def mavenhome = tool 'maven'
env.PATH = "${mavenhome}/bin:${env.PATH}"
}
stage('clone'){
git branch: 'master' ,
credentialsId :'5fdc9f01-d0b3-4305-bb38-e910fbb914a4' ,
url: 'https://github.com/ronnysss/Practice-Project.git'
}
stage ('Build'){
sh '''
cd Java-project
mvn clean install '''
}
}
