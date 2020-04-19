# IT-Ops Automation : 

<p align="center"

 ![ansible](https://user-images.githubusercontent.com/55547108/79690541-9bcfe180-8278-11ea-9cbc-eaf34e6bae62.png)

</p>
  
  ### This Repository is Intended to Provide the Installation steps & Ansible roles for AWS(Amazon-Web-Services) and its Services.

#### Roles :

 - EC2-Instance with desired Availablity Zone's
 - EC2-Keypair

#### Prerequisites :

 -   AWS user account
 -   Ansible
 -   Python
 -   Boto

#### Installation :

- Ansible :

>    - Install Ansible on a RHEL/CentOS Linux based system :
```shell 
           $ sudo yum install Ansible
```
>    - Install Ansible on a Debian/Ubuntu Linux based system :
```shell
           $ sudo apt-get install software-properties-common
           $ sudo apt-add-repository ppa:Ansible/Ansible
           $ sudo apt-get update
           $ sudo apt-get install Ansible
```        
>    - Install Ansible using pip :
```shell
           $ sudo pip install Ansible           
```

#### Once installed you can verify it by using : ```shell Ansible --version```

- Python :

```shell 
           $ sudo apt-get update
           $ sudo apt-get install python3.6
```

- Boto : 

>    -  First, install pip :
```shell   $ sudo apt install python3-pip or
           $ yum install python-pip
```
>    -  Now install boto :
```shell   
           $ pip install boto 
```
Ansible uses python-boto as a library to access API Calls. The boto pakckage needs **AWS credentials** in order 
to perform all the functions. The easiest way is to create a **.boto** file under your working **./home** directory:

```shell
           $ vi .boto
```

Then add the following:

```shell
          [Credentials]
          aws_access_key_id = <your_access_key_here>
          aws_secret_access_key = <your_secret_key_here>
```



