# Get local IP of client

Demo: https://cornips.github.io/getLocalIP

## Introduction

To identify clients in internal web systems it is sometimes useful to know its local IP address.
With this little JS (only 847 bytes gzipped), borrowed from [Daniel Roesler](https://github.com/diafygi/webrtc-ips), you can do this.

## Installation

```
npm install getlocalipjs
```

## Usage

Just make sure you have the following code in your HTML at the bottom:
```html
<!-- hidden iframe to bypass webrtc blocking -->
<iframe id="iframe" sandbox="allow-same-origin" style="display:none"></iframe>
<script src="dist/getlocalip.min.js"></script>
<script>
    getLocalIP(function(ip){
        console.log(ip);
    });
</script>
```
