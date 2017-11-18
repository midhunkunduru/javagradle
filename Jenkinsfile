node("master")
  def a = "Version"
  def b = "Application"
    
{
    stage("Checkout")
    echo "${Version}"
    echo "${Application}"
{  
    sh 'echo $BRANCH_NAME'
}
    
    stage("Build")
    {
        echo "Sample build"
        build job: 'parametertest/master', parameters: [string(name: 'Version', value: '1.1'), string(name: 'Application', value: 'html')]
    }

}
