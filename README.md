# How to Install Genymotion & VirtualBox on Parrot OS

I've recently dived into the world of "hacking". No, not the type of advanced hacking that you see in Watch Dogs or Mr. Robot, because I am a super noob/skiddie, and let's be honest, cybersecurity is vast and difficult to get started in. So I thought, why don't I document my progress or learning milestones by helping others with simple things whilst I climb the ranks from skiddie to _"I now know how to not breakdown every time I use Burp Suite"._

![Mr Robot Crying](https://media.giphy.com/media/JFo3BEQFmK4cU/giphy.gif)

When you're ready, grab your closest Red Bull and your favorite cool-guy shades, and let's dive into this tutorial on how to install [Genymotion](https://www.genymotion.com/) & [VirtualBox](https://www.virtualbox.org/) on Parrot OS.

First, let's discuss why we would use Genymotion, and what VirtualBox is for. Genymotion is an Android emulator, meaning it emulates a mobile device via a VirtualBox (which allows us to run the Android OS on our operating systems). This emulation allows us to access real-time Android capabilities such as using the browser, downloading apps via the Play Store, or accessing the front/back camera - as we would with our actual device. We use device emulators for a variety of things, such as testing our Android apps that we made, or for android pen-testing. Now, a better method to test our apps is to use a rooted android device, and this requires a physical device, but that's a tutorial on its own. 

Now that we know what Genymotion and Virtualbox are used for, we can move on to the actual tutorial. Start up your Parrot OS system and open up your browser. Let's first download Genymotion.

## Genymotion Installation
First, we need to go to the Genymotion site and create an account. You need this account to be able to download and use Genymotion (obviously), so make sure you do that first. When you have done that, go to the following [link](https://www.genymotion.com/download/) and download the Linux (64-bit) version.

![Genymotion Desktop Download](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/nvh10kdz5xtqhrdu9ncg.png)

Once you have installed it, it will be in your Downloads folder. Open up your terminal using CTRL + ALT + T and let's cd into it.

![Terminal Genymotion](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ef2239taeamr42ts6hym.png) 
![Ierminal Genymotion](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/g27mf7bb2dsriezzts3y.png)
  
When we list all our files in our Downloads directory we can see that the Genymotion download file is there, but it is not accessible as we cannot execute it. _Remember, if you start typing the name of a file and press TAB, it will autofill, so save time using this._

![erminal Genymotion](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/hqk30vrnu524ojjmzu0x.png)

To change the file into an executable we use the command **chmod +x** and the filename. The chmod +x command adds x permission to a file or folder to change the file permission, thus making it executable.

![Terminal Genymotion](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/gfupqt8v5d0nmu12hp49.png)

Once we have changed it into an executable, we can now list all directories again and we can see that we have a new file that is now executable!

![Terminal Genymotion](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/mp2w59nvac0b473twn4u.png)
 
Let's now install our Genymotion. To do this we simply say **./filename**, which will be Genymotion. This will run the executable, and the installation will run. 

![erminal Genymotion](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/17pma5slb571d6e6pz3c.png)
 
Now that Genymotion is installed, we can open it up in our Applications Menu underneath Programming. Click on it, and it will open, but oops, we get an error! This is where Virtbualbox comes in.

![Terminal Genymotion](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/dk0m2iyeyugwocqxzvdb.png)

## VirtualBox Installation
To be able to use Genymotion, we need to install VirtualBox. Go to the following [link](https://www.virtualbox.org/wiki/Linux_Downloads), and download the relevant VirtualBox. I installed the **Debian 11** version. 

![Terminal VirtualBox](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/hlnyijr7smluwdf8s3gv.png)

Once it is installed, we need to move it to our Downloads folder to make things easier. To do this, just click on the folder icon in your Download history, and from there on move it to your Downloads.

![Terminal VirtualBox](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/9bj6hllyc09c897i0hzr.png) 
![Terminal VirtualBox](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ofy79i2pip009gfa0dpv.png)
 
Next, open up a new terminal using CTRL + ALT + T, and then you need to cd into your Downloads folder, just as before. From there on you need to run the **sudo apt-get update** command as stated in the documentation.

![Terminal VirtualBox](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/s8ufj35qw3eomeo8yxll.png) 
![Terminal VirtualBox](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/wtxrrdmdac2kd7y8pbz3.png)

After you have run the update command, then we can install Virtualbox using the **sudo apt install virtualbox** command. 

![Terminal VirtualBox](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/a7usvjjiv51e3mgorp38.png) 
![Terminal VirtualBox](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/twnpg8k71t1l0228c32s.png)

Voila, you have installed VirtualBox, and when we open up Genymotion again we can now see that it is working!

![Genymotion Setup](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/aohfs4zhloqeiagh7qdh.png)

## Genymotion Setup
Now that Genymotion and VirtualBox are installed, we can now sign in and get our first virtual device up and running. 

![Genymotion Setup](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/kx03fuvq6er1jat1s7mu.png)
![Genymotion Setup](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/5rhwcdcq10t62n6jn3zw.png)
![Genymotion Setup](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/fmom9fehylah562uq33b.png)
![Genymotion Setup](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/lhxx5wkqikyo33cgit4n.png)
![Genymotion Setup](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/nu3tyx4l8q80keb84qt0.png)
![Genymotion Setup](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/kofgkc8v5pwl3ft1vpk1.png)
![Genymotion Setup](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/hpzlteeyb1jiuom2oe3i.png)
       
Okay, that's a wrap. I hope that this tutorial helped you, and was not too complex. See ya' next time!



