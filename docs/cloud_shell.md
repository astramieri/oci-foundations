# Oracle Cloud Shell

Cloud Shell is  a small virtual machine running a Linux shell which you access through the browser through the OCI Console. And it comes with a pre-authenticated OCI CLI and lots of utilities like Git, Java, Python, etc.

SSH protocol, also referred to as **Secure SHell**, is a method for secure remote login from one computer to another. 

## Generate SSH key pair

    (shell)$ mkdir .ssh
    (shell)$ cd .ssh
    (shell)$ ssh-keygen -b 2048 -t rsa -f mykeyname

## Image and Shape

Shape is basically a (virtual hardware) template which determines number of CPUs, amount of memory, other resources. 

Image is basically an operating system, which runs on top of that shape.



