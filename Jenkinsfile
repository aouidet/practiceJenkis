@Library('my_shared_library@main') _

properties([
    parameters(
          [
            file(
                    description: 'please browse your desk and select the file you want to upload.',
                    name: 'uploadedfile'
                )
          ]
        ),
        disableConcurentBuilds(),
        buildDiscarded(
                logRotator(
                        artifactDaysToKeepStr: '',
                        artifactNumTokeepStr: '',
                        daysToKeepStr: '7',
                        numToKeepStr: '10'
                    )
            )
    ])
node {
   sh "echo ${uploadedfile}"
   def file_in_workspace = copy_bin_to_wks.inputGetFile('text.txt');
   sh "ls -ltR"
   sh "echo ${env.WORKSPACE}"

   sh "echo ${file_in_workspace}"
}