# Remote Access From Your Computer to ieng6

## **Step 1) Installing Visual Studio Code**


Go to the [Visual Studio Code website](https://code.visualstudio.com/) and install Visual Studio Code for your operating system. Follow what the site and installer tell you to do. 

Once it is setup open up Visual Studio Code and your screen should look like this. 

![Pic1](LabReport1Pic1.PNG)

## **Step 2) Connecting Remotely**


Before going any further if you are on a Windows device you will need to install [OpenSSH](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse).

Now for everyone, go find your [CSE15L course specific account](https://sdacs.ucsd.edu/~icc/index.php).

Look for the account that is in the form of **cs15lsp22zzz** (The z is an actual letter but varies from account to account).

Now you will go to Visual Studio Code and open up a new terminal by clicking on ```Terminal``` and then on ```New Terminal```.

Now you will type ```ssh cs15lsp22zzz@ieng6.ucsd.edu``` (using your course specific account instead of the zzz). A message will then pop up.

> Are you sure you want to continue connecting (yes/no)? 

Type yes and then you will be prompted to type your password. Do so and your terminal should look something like this. 

![Pic2](LabReport1Pic2.png)

## **Step 3) Running Some Commands**

Here are some commands that you can try running in the terminal. 

- ls

- ls -a

- cd

- pwd

- mkdir

- touch

- cat 

- cp

Here are some examples of how to call these commands and what the output should look like!

![Pic3](LabReport1Pic3.PNG)
## **Step 4) Moving Files With `scp`**
Now we will be copying some files from our computer to ieng6. You can do this with many files on your computer, but for this we will be using a basic example just to show you how it works. 

First of all you can copy this code bellow, put it into a directory of your choice, and then run it using `javac WhereAmI.java; java WhereAmI`
```
class WhereAmI {
    public static void main(String[] args) {
        System.out.println(System.getProperty("os.name"));
        System.out.println(System.getProperty("user.name"));
        System.out.println(System.getProperty("user.home"));
        System.out.println(System.getProperty("user.dir"));
    }
}
```
