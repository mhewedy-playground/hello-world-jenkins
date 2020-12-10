//@Library('wolox-ci') _

library identifier: 'wolox-ci@master', 
        retriever: modernSCM([$class: 'GitSCMSource', remote: 'https://github.com/mhewedy/wolox-ci.git'])

node {
  checkout scm
  woloxCi('.pipeline.yml');
}
