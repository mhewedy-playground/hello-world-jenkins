library identifier: 'wolox-ci@use_image_instead_of_dockerfile', 
        retriever: modernSCM([$class: 'GitSCMSource', remote: 'https://github.com/mhewedy/wolox-ci.git'])

node {
  checkout scm
  woloxCi('.pipeline.yml');
}
