This is the notepad for github actions certification course

1. Every Jobs must run on a runner, so when we create a job We may specify the tag *runs-on*

## MODULE 2

**lesson 4:**

You can create your own github actions and publish inside the repo avoiding to deploy on github actions marketplace
To know if an actions was create by github team

- name: Checkout
  uses: actions/checkout@v4.2.0
  The name has the word actions if **actions** word is not present, the action was developed for an user
- name: FTP Deploy
  uses: SamKirkland/FTP-Deploy-Action@v4.3.5

**lesson 5:**

On this lession, We create a new yaml file, and there We define some steps to instal curl packages, in the last step, We call a .sh file where We defined how to install curl packages

**lesson 6:**

We used defined actions from github marketplace, one of them were node setup and php action.
We learn how to use and configure actions from marketplace

**lesson 7:**

Reuse Actions, this video explains how to create actions for other actions and developers and how to call them.

**lesson 8:**

We learned how to send and get parameters for githubactions reuse

To get a parameter, we must add inputs section:

```
inputs:
  message:
    description: "Message file description"
    required: true
    default: "Hello this is this is the default message"
  folder-name:
    description: "Folder name"
    required: true
    default: "folder"
  file-name:
    description: "File name"
    required: true
    default: "file.txt"


```

For send parameters, We must add with parameter after call reusable workflow

Lesson 9:

Working with services, services are based on docker images. We can pull a docker image from docker registry and work with it on my workflow
