node{
             stage('checkout')
                            {
                         echo 'Hello, git'
                         git 'https://github.com/ElferjeniDevops/maven/'
                        }
                
             stage('Example Build') 
                          { 
                          echo 'Hello, Maven'
                          bat 'mvn --version'
                        }
             stage('phase de validation de code') 
                          { 
                          echo 'phase de validation de code '
                          bat 'mvn validate'
                        }
             stage('phase de compilation') 
                          { 
                          echo 'phase de compilation '
                          bat 'mvn compile'
                        }
             stage('phase de tesT') 
                          { 
                          echo 'phase de test '
                          bat 'mvn test'
                        }
             stage('phase de packetage') 
                          { 
                          echo 'phase de packetage  '
                          bat 'mvn package'
                        }
             stage('phase d_intallation de pachake dans votre RL') 
                          { 
                          echo 'phase d_intallation de pachake dans votre RL '
                          bat 'mvn validate'
                        }
               stage('phase de deploiement d_un artefact dans le referentiel distant') 
                          { 
                          echo 'phase de déploiement d_un artefact dans le référentiel distant'
                          bat 'mvn deploy'
                        }
 }
      
     
