# jenkins-2.289.1_plugins


This repository contains all the basic plugins for the jenkins. 


These plugins were stored in the github using git lfs 


To install git lfs command follow below steps: 
-------------------------------------------------

1) download git lfs for your operating system https://git-lfs.github.com/
2) once downloaded change directory to the path where the git-lfs is downloaded : cd Downloads/git-lfs-darwin-amd64-v2
3) now run the script:  ./install.sh

first change directory to your project dir/repo: Jenkins-2.289.1_plugins and follow below steps: 
-----
take a backup of that copied plugins directory from ACG sandbox

rm -r */                                        delete all the directories

find . -type f ! -name '*.jpi' -delete          Find and delete all non matching files except .jpi files

now zip the file you want to upload to github.

git clone the repository where you want to upload and copy and add commit. 

git lfs install   

git lfs track plugins.zip

git add .gitattributes

git add plugins.zip

git commit -am "uploading jenkins plugins"

git push 

https://docs.github.com/en/github/managing-large-files/versioning-large-files/configuring-git-large-file-storage

copying from ACG sandbox to my macbook: 
------------------------------------------
scp -r cloud_user@932f5e74051d.mylabserver.com:/var/lib/jenkins/plugins /Users/sagarchamlagai/Downloads/plugins_jk/.
