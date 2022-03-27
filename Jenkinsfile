@Library('my_shared_library@main') _

node {
   def file_input = sh "echo ${uploadedfile}"
   def file_in_workspace = copy_bin_to_wks.inputGetFile(file_input);
   sh "ls -ltR"
   sh "echo ${env.WORKSPACE}"

   sh "echo ${file_in_workspace}"
}