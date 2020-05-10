## Welcome to Ansible project

1. what this project does?

~  This project does configure the following tasks:

       a) install jenkins servers.

       b) Rhel 8 iso yum configuration.

       c) pull the docker images that you want from the dockerhub ( only those that don't require you to login ).

       d) some additional tasks such as screen resolution inside virtualbox vm of rhel 8.
 
       e) It will also install jupyter and some python libraries used for machine learning projects.

       f) all you need to configure the roles according to your requirements.

## What are prequsites?

       a) Ansible must be installed.
      
       b) All the controlled nodes must have given ssh key access for login and don't require the passwords.

       c) Controller node must have entry in thier host files with the alias for the remote nodes as the file is at /etc/hosts and entry should be like:
       `127.0.0.1   localhost localhost.localdomain localhost4 localhost4.localdomain4
        ::1         localhost localhost.localdomain localhost6 localhost6.localdomain6

## How to use?
```markdown
       1. Go to the inventory file ( hosts ) in your current directory:         
       To install jenkins: 
       a) Change your inventory file from such that:
       `[jenkinsservers]
        localhost`

                   To

       `[jenkinsserver]
        server1
        server2
        server3`
         

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for


Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Chandrashekhars816/ansible-projects/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
