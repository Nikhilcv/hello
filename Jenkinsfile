pipeline{
       agent none        
                    stages{
                           
                   
               stage('fromgit')
                    {
                           //def anil = 'M4'
                           agent{
                           label "slave"
                           }
                  steps{
                        git 'https://github.com/Nikhilcv/hello.git'
                         withEnv(["PATH+MAVEN=${anil}/bin"]){
                         sh 'mvn clean package'
                        sh 'scp /home/nikhil/jenkins/workspace/hello/target/webapp.war root@192.168.7.138:/home/nikhil/softs/tomcat7/webapps'
                               }
                    }
                  }
           }
}
