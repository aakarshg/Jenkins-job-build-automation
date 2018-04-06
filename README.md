# Jenkins job build automation

### Installing jenkins
The script ans.yml contains script to install jenkins and other dependencies necessary to create the job and build the job


#### INSTRUCTIONS
* Edit the inventory file with the IP address and also reflect same changes everywhere else
* Place the ssh key in the directory and update the inventory file accordingly
* To run the script please run : `ansible-playbook -i inventory ans.yml -s`

#### NOTE:
* The config.xml and jobs.xml has been downloaded through transfer.sh and the files are available for 14 days. 
* We can also use copy/template to share the xml files.


### Screencast
Here's the link to screencast: ![gif](https://github.com/aakarshg/Jenkins-job-build-automation/blob/master/final.gif)
