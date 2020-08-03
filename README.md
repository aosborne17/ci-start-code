# Why should we use SSH with Git-hub

## SSH keys and Git-hub
### There are two methods to clone the repo

``` SSH AND HTTPS ```
- We have two types repos ```public repo``` 
- second is ```private repo```

There are two methods
 to clone a repository, SSH and HTTP

With public repositories, anybody can fork our code and use it, thus meaning it is not secured

Do avoid this we can make our repo private, meaning our work would be restricted to certain people

- generate SSH keys on your local system
- copy the key from local system to the specific repo on git-hub (ci-start-code)
-.ssh key folder where the ssh keys are available
- name new key as your name andrew

Once in Users/asbo
``` cd .ssh ```
then run in the below command, adding in your email address
``` ssh-keygen -t rsa -b 4096 -C "AOsborne@spartaglobal.com" ```

When prompt with the question "Enter file in which to save the key (/c/Users/aosbo/.ssh/id_rsa):"
enter your name

We then press enter twice to input an empty passphrase and we should be given a key fingerprint

If we run the command ``` cat andrew.pub ``` will give us our public key

We then copy the key and go to settings on the repo we have created and go to the
deploy keys

We then click add deploy key and name the key our name

![Deploy Key](images/)
post pick here