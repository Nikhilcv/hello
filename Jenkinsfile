pipeline{
       agent any
             stages{
               stage('fromgit')
                    {
                  steps{
                        git 'https://github.com/Nikhilcv/hello.git'
                        sh 'mvn clean package'
                        sh 'scp /target/com/rns/app/webapp.war root@192.168.7.138:/home/nikhil/softs/tomcat7/webapps'
                               }
                    }
                  }
           }
