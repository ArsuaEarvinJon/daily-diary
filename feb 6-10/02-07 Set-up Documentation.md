# Set-up Documentation
*February 7, 2023*

## **General List**

- SSH Public Key
- Python
- Python Virtual Environment
- Mockoon and Mockoon CLI
- IntelliJ IDEA Community Edition

---

### **SSH Public Key**

SSH, or secure shell, is an encrypted protocol used to administer and communicate with servers. When working with an Ubuntu server, chances are you will spend most of your time in a terminal session connected to your server through SSH.

### *1. Creating Key Pair*

    $ ssh-keygen

Output:

    Generating public/private rsa key pair.
    Enter file in which to save the key (/home/earvin/.ssh/id_rsa): 
    Enter passphrase (empty for no passphrase): 
    Enter same passphrase again: 
    Your identification has been saved in /home/earvin/.ssh/id_rsa
    Your public key has been saved in /home/earvin/.ssh/id_rsa.pub
    The key fingerprint is:
    SHA256:SDzCReVuYMRk2LW0M1jQ0dD8K8EJBR8TaBs/972tiAw earvin@administrator-System-Product-Name
    The key's randomart image is:
    +---[RSA 3072]----+
    |     *B=OX=.     |
    |   ..=o=*++o     |
    |    o B.**.o     |
    |     + =.o* o    |
    |      . S  + o . |
    |       .  . . . .|
    |        E  .    o|
    |         o . . ..|
    |          o . .. |
    +----[SHA256]-----+

*Note: should there be no modifications in file directory and passphrase, press enter in intended inputs*

### *2. Manual Copying of Public Key*

    $ cat ~/.ssh/id_rsa.pub

Output:

    ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCq0TMgM7Cco0X9Mg5yPeZLdlMdgWwsPLBRpblaCVZ74kLgJ55n2Cyu5yKb3vJGvz4R8IOhDL+odM+pZtOsxmJGGtZhriAyDi+uhr9+xPtsNd6NYqMaAsoQH5vY4rkaF+j/+jl7/y14JB5FdI14+1LDvQKiEfqLCcVx9lnoTcD3tmX7BxT/Xuq1EPx1I8OddvXJG2iq6c1/Z21/7ThdWWEhNnAUkflbTFMCVUivcYKXtQ7jqvGNw/LBCK91psxRrZQWGsCgMGww0Lw2PTtmSZE9t6THKsEGO6TebCuhOT2u9GiYQqVxX4Pw1hdhTp2zIFlelvrc7hDwtkW7MLFH3ufQJ5RwxLBNIG+CaZsaScWzCohvk0QqwNDix87GQ7VmxxooPwh7E2sQm1ZiQsHbx/780u5UHqyig8yGjrwSrluhaEG8bsL8EvrcxnxESj4Fnxi+dzLsoHBiQK4Cdu5nGktczGUE5pi/7uOzLF7Dnq5QiYM4RAvD74jbiaQ2xaE60ek= earvin@administrator-System-Product-Name

---

### **Installing Python**

    $ sudo apt install python3

*Note: Terminal will ask for user password to proceed with sudo*

APT will automatically install Python

---

### **Python Virtual Environment**

*Creating the environment*

    $ sudo python3 -m venv {name_of_project}

*Activating the environment*

    $ source {name_of_project}/bin/activate

*deactivating the environment*

    deactivate

---

### **Installing Mockoon and Mockoon CLI**

Install Mockoon

    $ sudo snap install mockoon

Install Mockoon CLI

    $ sudo npm install -g @mockoon/cli

---

### **Installing IntelliJ**

*What is IntelliJ IDEA?*

IntelliJ is an integrated development environment for software development in Java, Kotlin, Groovy, HTML, etc.

1. Download [IntelliJ IDEA Community Edition](hhttps://www.jetbrains.com/idea/download/download-thanks.html?platform=linux&code=IIC)
2. Extract the downloaded file.

3. Open terminal and cd into "{installation_directory}/bin"

        $ ./idea.sh

*Additional: Creating IntelliJ IDEA shortcut o desktop*

    1. Execute instructions above.
    2. Once opened, click the "gear icon" located in the lower left of the welcome page.
    3. Click "Created Desktop Entry"


