node("master")
      def a = "Version"
  def b = "Application"
{
    stage("Checkout")
  
    
{  
    sh 'echo $BRANCH_NAME'
  echo "${Version}"
    echo "${Application}"
}
    
    stage("Build")
    {
        echo "Sample build"
        build job: 'parametertest/master', parameters: [string(name: 'Version', value: '1.1'), string(name: 'Application', value: 'html')]
    }

}
