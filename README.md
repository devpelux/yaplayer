# YouTube APlayer
Do you need to play audio from a YouTube video?  
You can use this little plugin. <br>

### How to use
1. Download source code from [latest release](https://github.com/firestormxyz/yaplayer/releases/latest).  

2. Load the files on your host provider.  

3. Insert the YouTube IFrame Player API.  

```html
<script src="https://www.youtube.com/iframe_api"></script>
```

4. Insert the javascript file.  

```html
<script src=".../yaplayer.min.js"></script>
```

5. Add a div element similar to this, with `id="youtube-audio"`...

```html
<div id="youtube-audio" data-video="VIDEOID" data-autoplay="0" data-loop="0" data-volume="100" data-startseconds="10" data-endseconds="20" data-theme="light" data-size="64"></div>
```

...where:  

***`data-video`*** is the **ID** of the YouTube video.  
***`data-autoplay`*** indicates to start playing audio immediately after the page loads (if is setted to `1`).  
***`data-loop`*** indicates to repeat audio continuously (if is setted to `1`).  
[***OPTIONAL***] ***`data-volume`*** changes audio volume between `0` to `100`.  
[***OPTIONAL***] ***`data-startseconds`*** is used to set the time where the audio will begin playing (in seconds).  
[***OPTIONAL***] ***`data-endseconds`*** is used to set the time where the audio will end playing (in seconds).  
[***OPTIONAL***] ***`data-theme`*** is used to set the theme of the audio player (`light` or `dark`).  
[***OPTIONAL***] ***`data-size`*** is used to set the size of the audio player (in pixels). <br><br>

### Loading by CDN
If you want, is possible to loads the files from GitHub, by any cdn provider (for example *jsDelivr*).  
Simply insert this tag `<script>` instead of the previous one:  

```html
<script src="https://cdn.jsdelivr.net/gh/firestormxyz/yaplayer@1.0/minified/yaplayer.min.js"></script>
```

Then add the extra ***`data-loadfrom`*** parameter to the loading `<div>`:  

```html
<div ... data-loadfrom="https://cdn.jsdelivr.net/gh/firestormxyz/yaplayer@1.0/minified/" ... ></div>
```

In this way both the javascript file and the svg images will be loaded from GitHub. <br><br>

### Demo
You can see a demonstration here: [https://fire-space.weebly.com/yaplayer.html](https://fire-space.weebly.com/yaplayer.html) <br><br>

### License
By firestormxyz (Salvatore Peluso)  
Licensed under The Unlicense.

<a href="https://github.com/firestormxyz/yaplayer/blob/master/LICENSE"><img title="Licensed under The Unlicense" width="32" src="https://upload.wikimedia.org/wikipedia/commons/6/62/PD-icon.svg"></a>
