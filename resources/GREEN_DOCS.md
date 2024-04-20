# Team 5: Team 5 Green Team Documentation

This document is intended to be used by the green team for using our (Team 5's) services.

## Using the File Service Over SSH

### If You're on Linux...

Firstly, open a terminal.

![Image of an open terminal](img/TERM.png)

Next, type the following:

```sh
ssh {your user name}@files.team5.isucdc.com
```

> Replace `{your user name}` with your username.  
> Press enter once the command looks good.

Next, type in your password.

> NOTE: your password will be invisible as you type it, but rest assured, it is being received.

You are now logged in.

### If You're on Windows...

> We will use the ssh client PuTTY as an example of how to access this service.
> There are many other ssh clients available for windows, but the process is very much the same.
> 
> We will begin assuming that PuTTY is open.

First, put `files.team5.isucdc.com` in the ___ box.

>> Next documenter: please note and screenshot the buttons to press
>> also, please take many screenshots.

TODO: Image.png

-Tell how to enter username and password.

TODO: Image.png

-Tell that they are in

### Now That You've Logged in

Your files are now available for your perusal through the command line.
You have the ability to execute basic commands like `ls`, `mv`, `rm`, `cp`, etc.
You also have the ability to run the editors `nano`, `vim` and `emacs`.

### Using the File Service as an Admin over SSH

Firstly, follow the instructions above ([Using the File Service](#using-the-file-service)) to log in.

Everything will be the same until you need to run a privileged command.

Let's use the example of updating the system using `dnf`.

To do this you will run:

```sh
sudo dnf upgrade
```
Then enter your password when prompted.

> Note: Like when you log in over ssh, your password will be invisible as you type it, but rest assured, it is being received.

## Accessing the Website

Open your web browser and go to the following website:

```
www.team5.isucdc.com
```

You should get a site that looks like this one:

![The highschool website](img/COUNTRY_ROOOOOADS_TODD_ME_HOME.png)

### Adding yourself to the mailing list

First, go to the website. This is explained directly above this section.

Next, click the button labeled `ENEWS` on the green ribbon.

![The button "ENEWS" is verry happy.](img/FLYY_ME_TO_EEE_NEWS_LET_ME_PLAY_AMONG_DOT_TARS.png)

Next, enter your email in the box below the text `Enter email to sign up for eNews`.

![The email "joe.shmoe@example.com" has been entered into the text box](img/HI_IM_JOE_SHMOE!!.png)

Finally, click the `SEND` button.

![The button "SEND" is verry happy.](img/JOE_GETS_PWNED.png)

## Using the Windows Client

TODO: EXAMPLE OF AN RDP CLIENT

-The user enters their info.

-The user is on teh windowes client.

### Using RDP
![Click the windows button and start typing "Remote Desktop Connection" to search for the RDP client.](img/rdp_doc_1.png)

![When the window appears, type in the hostname of the computer you wish to connect to.](img/rdp_doc_2.png)

![Click "Show Options" in the bottom left corner, and enter your desired username. Click "Connect".](img/rdp_doc_3.png)

![Enter the password for the desired user and the process is complete!](img/rdp_doc_4.png)

### Accessing Your Files From the Windows Client

Now that you are on the machine, open the start menu.

![An arrow pointist towards the bottom left of the screen.](img/STARTING_ARROW.png)

Next, type `CMD` into the start menu.

![The word 'CMD' has been entered into the start menu's search box.](img/PRESS_COMMAND.png)

Select Command Prompt.

![The option "Command Prompt" is selected from the start menu.](img/SELECT_COMMAND.png)


A friendly text window should pop up.

In this window type the following:

```bat
net use Z: \\files.team5.isucdc.com\homes /user:{username}
```

> Replace `{username}` with your username.

Press enter once what you typed looks good.

When prompted, enter your password.

> Note: Your password will be invisible as you type it, but rest assured, it is being received.

Your files are now mounted as the `Z:` drive and can be interacted with however you please.

Remember to log off of the windows client when you are done, to ensure that no one can maliciously modify your files.

## Using the Linux Client

TODO: COPY FROM [THIS](#using-the-file-service-over-ssh)
