@Library('my_shared_library@main') _

node {
   sh "echo ${uploadedfile}"
   def file_in_workspace = copy_bin_to_wks.inputGetFile('text.txt');
   sh "ls -ltR"
   sh "echo ${env.WORKSPACE}"

   sh "echo ${file_in_workspace}"
}