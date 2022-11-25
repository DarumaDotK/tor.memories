# Tor Browser to ubuntu 22.04
I documented a problem using Tor Browser on unbutu 22.04 here.

we will manually download the latest version of the Tor browser from its website. _[Here is the link to visit.](https://www.torproject.org/download/)_ On the page click on the Linux edition.

NOTE : For me in today `tor-browser-linux64-11.5.8_en-US.tar.xz`

then

![pic1](/src/Screenshot%20from%202022-11-25%2010-03-16.png)

~~~
cd Downloads

tar -xvf tor-browser-linux64-xx.x.x_en-US.tar.xz

cd tor-browser_en-US/

./start-tor-browser.desktop --register-app
~~~

Copy Browser shortcut to Desktop

![pic2](/src/Screenshot%20from%202022-11-25%2010-02-10.png)

~~~
cp start-tor-browser.desktop ~/Desktop

cd ~/Desktop

gio set ~/Desktop/start-tor-browser.desktop metadata::trusted true

chmod a+x ~/Desktop/start-tor-browser.desktop
~~~

All done

![pic3](/src/Screenshot%20from%202022-11-25%2010-00-40.png)
