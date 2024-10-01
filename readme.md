This is the notepad for github actions certification course

1. Every Jobs must run on a runner, so when we create a job We may specify the tag *runs-on*

Module 2
 
lesson 4:
 You can create your own github actions and publish inside the repo avoiding to deploy on github actions marketplace
 To know if an actions was create by github team
     - name: Checkout
	    uses: actions/checkout@v4.2.0
 The name has the word actions if **actions** word is not present, the action was developed for an user
           - name: FTP Deploy
            uses: SamKirkland/FTP-Deploy-Action@v4.3.5

lesson 5:
 On this lession, We create a new yaml file, and there We define some steps to instal curl packages, in the last step, We call a .sh file where We defined how to install curl packages
