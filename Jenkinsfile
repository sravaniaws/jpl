node
{
    stage ('GIT')
    {
        git 'https://github.com/sravaniaws/jpl.git'

    }
    stage ('Package')
    {
        sh 'cd jpl' && 'mvn package'
    }
    stage ('archiveArtifacts')
    {
        archiveArtifacts 'target/gameoflife*.zip'
    }
}
