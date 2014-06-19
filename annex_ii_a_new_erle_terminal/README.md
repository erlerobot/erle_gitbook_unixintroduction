# Annex II: A new Erle terminal
---

Sometimes, when you are working with *Erle* is confortable having more than one terminal.
In this annex, you are going to learn how to **connect Erle and your computer** and how to launch as many erle terminals as you wish.

####Connecting with Erle

Connet Erle to your computer, using the USB wire.

Open a terminal an type:
```
ls /dev
```
Whenever you connet a device to your computer, that device appears in this list.Here is erle:
**imagen**
This is only a verification of erle conectivity.

In the same terminal type:
```
ifconfig
```
You get this in the screen:
**imagen**


Usually en0 and en1 correspond to internet connection, bridge are usually matter of a virtual machine... We now care about *en4*, which is related to erle (you can check that  the status is active when erle is connected).

Now open a erle-terminal and type:
```
ifconfig
```
You get this:
**imagen**

There you can read in the usb0 section the *erle conection id*:
```
inet addr:11.0.0.1
```
At this point we are going to make en4 work in the same id that erle does. We are going to make them work in the same sub-network.
Type in your computer terminal:
```
sudo ifconfig en4 11.0.0.2
```

You can check they (erle and your PC) are connected by tipping in your computer terminal:
```
ping 11.0.0.1 (erle id)
```
The result should be something like this:
**image**

#### A new Erle-terminal

After doing the process above, you can launch as many shells as you want in a simply way. We are going to use ssh command in the computer terminal, which lests you logging into a remote machine and executing commands on that machine.
The syntaxis is easy:

```
ssh usuario@id
```
In our case:
```
ssh root@11.0.0.1
```
####Transferring files from your computer to Erle

Once you have your computer and erle connected, for transferring a file from your pc to erle's home, type:
```
scp file root@11.0.0.1~/
```
Note: `scp` is similar to `cp`, is something like *a copy through the network *
Let's see an example:
