# c-workspace

---
<br/>

## Getting started with C

This repository is intended to understand the development workflow and all nity gtries of C language.


---

## All the learnings would be placed in this ReadMe.md file :


*  To compile the file you would need a compiler usually 'gcc' works the best and is recomended for beginers.

* More on **gcc** can be read [here.](https://www3.ntu.edu.sg/home/ehchua/programming/cpp/gcc_make.html)

* To install gcc there are different options for different operating systems :

    * For windows please navigate [here](https://www3.ntu.edu.sg/home/ehchua/programming/howto/Cygwin_HowTo.html).
    * For mac os please install XCODE ide from app store which will inturn install gcc as well.
    *  For linux different OS have differnt package managers which can install the basic development tools for working with C language :

        * Ubuntu :
        ```
            sudo apt update
            sudo apt install build-essential
        ```
        *  Fedora :
        ```
            dnf groupinstall 'Development Tools'
        ```
        * RHEL/CentOS
        ```
            yum groupinstall 'Development Tools'
        ```
        * Manjaro
        ```
            pamac install gcc
            pacman -S gcc
        ```
        * Arch Linux
        ```
            pacman -Sy gcc
        ```

* Once you have the compiler just use that to compile the C program using below command :

```
gcc -Wall hello.c -o hello

```

* This will enable all compiler's warning messages and help developer. hte -o option is to specify the output fileanme, if not used a file with a.out is generated as output. Please refer [here.](https://www.geeksforgeeks.org/compiling-a-c-program-behind-the-scenes/) for more.

* Run the compiled binary file as below : 

```
./hello

```


---


### Compiling using Make

* Compiling manually is a good first step but as soon as the code grows compiling manually doesnot make sense and one has to do this using tools such as Make and CMAKE.

* checkout the basic ```Makefile``` written in the basics folder.
* The ```make build``` command runs the compilation process and creates a binary in target folder
* The ```make run``` command runs the binary created in the above command.
* The ```make clean``` command removes the binary created in the above steps.

