# digital-display-webpage
A couple of html pages to display content on a digital display, tested with a Raspberry Pi 2

Using Screenly-OSE https://www.screenlyapp.com/ose/ I set it to load index.html, and reload every 1000 seconds by adding a blank.html page for 1 second in the asset list (crashed otherwise, memory leak perhaps)

Put index.html and slideshow.html in a folder on your webserver (or on the digital display computer)

Create a folder called photos in that folder

Copy photos to that folder

Create photolist.txt in the same folder as slideshow.html, a list of filenames of photos in the photos folder

I use this Windows command:

dir photos\*.jpg;photos\*.png /b > photolist.txt
