pipeline{

agent{

label{

label 'label-172.31.37.80'
customWorkspace  '/mnt/pipeline'
}
}


stages{

stage('install httpd'){

steps{

sh"yum install httpd -y"
}
}

stage ('deploy index.html'){

steps {
 sh"cp -r index.html /var/www/html"
}
}

stage('restart httpd'){

steps {

sh "service httpd restart"
}
}
}
}


