stage('build') {
      cmd_exec('echo "Buils starting..."')
      dir("build_folder"){
      bat "run.bat"
  }
}

def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
