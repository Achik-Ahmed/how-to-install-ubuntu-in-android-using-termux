# How to Install Ubuntu in Android Without Root (Easy Steps)

![how to install ubuntu in android](https://github.com/Achik-Ahmed/how-to-install-ubuntu-in-android-using-termux/blob/main/how_to_install_ubuntu_in_android.jpg)

Hey there! 
Did you know that you can install and run Ubuntu on your Android phone without rooting it? Well, the answer is YES! You can install and use Ubuntu on your Android just like a mini-computer, and the best part is you need to root your Android phone.

In this post, I will share how you can install Ubuntu 22 on your Android phone using **Termux**, and also how to use the Ubuntu GUI like a real desktop with the help of the **VNC Viewer app**.

> 🔗 [Read Full Blog Post with Images & Commands](https://www.achik.us/how-to-install-ubuntu-in-android-without-root/)

## What is Ubuntu?

Ubuntu is a free and powerful Linux operating system. It’s used by developers, hackers, students, and even companies. Now you can use it on your Android phone too — without any special tricks, just with some simple steps.

## What You Need

Before installing Ubuntu, make sure you have these:

- Android Phone (Android 7.0 or above)
- At least 5 GB Free Storage
- At least 2 GB RAM (4 GB recommended)
- Good Internet Connection (1–2 GB data needed)
- Termux latest App (from F-Droid or GitHub)
- VNC Viewer App (for GUI interface — optional)

## How to Install Ubuntu in Android

Here are the steps to **install Ubuntu in android without root**:

### Install Termux
Download it from F-Droid or GitHub (not from Play Store).

### Update Termux  
```bash
apt update && apt upgrade -y
```

### Install Required Packages  
```bash
pkg install wget curl proot tar -y
```

### Download Ubuntu Installer Script  
```bash
Read -the full blog article.sh
```

### Run the Script  
```bash
chmod +x ubuntu22-xfce.sh && bash ubuntu22-xfce.sh
```

> During setup, set a 6-digit VNC password when asked.

That’s it! Ubuntu will now install. Wait patiently.

## How to Use Ubuntu GUI on Android

If you want to use Ubuntu like a desktop with buttons, mouse, etc., follow these steps:

### Start Ubuntu
```bash
./start-ubuntu22.sh
```

### Start VNC Server
```bash
vncserver
```

### Open VNC Viewer App  
Set:

- Address: `localhost:5901`
- Name: `Ubuntu`

Enter the password you set earlier and connect.

Boom! Now you're inside Ubuntu GUI on Android.

## How to Stop Ubuntu or GUI

- Stop GUI:  
```bash
vncserver -kill :1
```

- Exit Ubuntu:  
```bash
exit
```

---

## How to Start Again Next Time

Whenever you want to start Ubuntu again:

```bash
./start-ubuntu22.sh
vncserver
```

Then connect using VNC viewer again. Simple!

## How to Uninstall Ubuntu

If you want to remove everything:

```bash
rm -rf ubuntu22-fs ubuntu22-binds start-ubuntu22.sh ubuntu22-xfce.sh
```

Done! Everything is cleaned up.

## Read Full Article

To get detailed steps with pictures, commands, and setup screenshots, check out the full blog post 
 **[Read Here](https://www.achik.us/how-to-install-ubuntu-in-android-without-root/)**

Thanks for reading! If you like it, don’t forget to ⭐ this repo and explore more tools on my blog!
