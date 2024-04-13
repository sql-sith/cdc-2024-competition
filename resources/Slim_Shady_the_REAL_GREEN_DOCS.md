# Team 5: Team 5 Green Team Documentation

This document is intended to be used by the green team for using our (Team 5's) services.

## Using the File Service Over SSH

### If You're on Linux...

Firstly, open a terminal.

TODO: TERM.png

Next, type the following:

```sh
ssh {your user name}@files.team5.isucdc.com
```

> Replace `{your user name}` with your username.

Next, type in your password.

> NOTE: your password will be invisible as you type it, but rest assured, it is being received.

You are now logged in.

### If You're on Windows...

TODO: Windows SSH client example.

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

### Adding yourself to the mailing list

First, go to the website. This is explained directly above this section.

Next, click the button labeled `ENEWS` on the green ribbon.

TODO: IMAGE.png

Next, enter your email in the `BOXNAME` box.

TODO: IMAGE.png

Finally, click the `SUBMITNAME` button.

TODO: IMAGE.png


## Using the Windows Client

TODO: EXAMPLE OF AN RDP CLIENT

-The user enters their info.

-The user is on teh windowes client.

### Accessing Your Files From the Windows Client

-Opens Commander

-netuse

-mounted as drive now

-can do things to the files

## Using the Linux Client

-SSH

-You're in...

##
