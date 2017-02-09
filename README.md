# HW1-B

Name: Aakarsh Gopi

Unityid: agopi

###Installing jenkins
The script ans.yml contains script to install jenkins and other dependencies necessary to create the job and build the job


####INSTRUCTIONS
* Edit the inventory file with the IP address and also reflect same changes everywhere else
* Place the ssh key in the directory and update the inventory file accordingly
* To run the script please run : `ansible-playbook -i inventory ans.yml -s`

####NOTE:
* The config.xml and jobs.xml has been downloaded through transfer.sh and the files are available for 14 days. 
* We can also use copy/template to share the xml files.


###Screencast
Here's the link to screencast: ![gif](https://github.ncsu.edu/agopi/HW1-B/blob/master/final.gif)

###Concepts

Q1. What are some benefits of continuous integration?

Continuous Integration is largely beneficical because it holds the following advantages:
* It ensures that the software is ready for deployment. Thus, allowing the deployment whenever it's necessary. 
* It makes it easier to detect any bugs and provisions to fix them quicker. 


Q2. What are some risks of not using continuous integration?

The biggest risks associated with not performing continuous integration is it's inability to produce testable builds. It has an adverse effect on other modules as well. The other major risks include:
* Struggles to maintain the environments in various phases.
* Wastage of time especially in the integration phases where redundant tasks have to be performed to send out code to testing teams
* Inability to test/build the software at any particular time
* Improbability associated with quick discovery of bugs.
* More importantly, it delays things because of the linear fashion in which things are done instead of doing it parallely.

Q3. What are some reasons why a company may use a dedicated build team?

Usually companies prefers to use a dedicated build team because of the following reasons:
* Reduction of operating costs associated with not having a build team to take care of build failures
* They serve as the incharge to work with configuration management 
* They are always there to take care of building verification scripts.
* To ensure that someone is tasked with building software.


Q4. What are some barriers to applying continuous integration in priorierty contexts?

There are a lot of concerns that can be heard in cases where continuous integration isn't adopted. Some of the major concerns that can be heard are:
* In cases of legacy application, it's difficult to transition to CI
* Costs associated with the building the infrastructure, which plays an important role in cases of small companies. Although, the initial investment is high, it should be noted that it saves a lot in the long run.
* Exorbitant size of code is usually a big barrier ex: Google
* Complex software which acts as hinderance because of lack of ease associated with automation

