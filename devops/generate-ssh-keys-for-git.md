### How to generate ssh keys for git

1. Open Terminal
2. `cd ~/.ssh`
3. `ssh-keygen -t rsa -b 4096 -C "email@example.com"`
4. Configure the key by inputting a password etc.
5. `id_rsa.pub`
7. Make sure your ssh agent is running by `eval "$(ssh-agent -s)"`
8. copy the key and paste it on **access keys** in bitbucket repo settings or in github keys.
9. Now clone the repo using ssh option. 

##### More
* [Github article](https://help.github.com/en/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
