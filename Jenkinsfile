node {
  stage 'Checkout Repository'
  git url: 'https://github.com/stackroute/sample-ci-project.git', branch: 'integration'

  stage 'Prune Dependencies'
  sh "npm prune"

  stage 'Install Dependencies'
  sh "npm install"

  stage 'Test'
  sh "npm test"
}