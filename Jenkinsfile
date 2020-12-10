library identifier: 'wolox-ci@development', 
        retriever: modernSCM([$class: 'GitSCMSource', remote: 'https://github.com/mhewedy/wolox-ci.git'])

node {
  checkout scm
  woloxCi('.pipeline.yml');
}
