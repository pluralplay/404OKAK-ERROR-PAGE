# okak 404 error page /w animation

## I don't claim that this is an ideal template, it was made using vibe-coding.

### Adaptation for mobile devices is a unfinished

![enter image description here](https://i.ibb.co/sJMPV4ZY/photo-2025-05-26-16-20-40.jpg)
Install:
- unzip archive on your site folder (errorpage folder in root site folder)
- edit your nginx.conf:
- add your server block here:

```
error_page 400 404 500 502 /error.html; #choice the error codes that this page will return and delete this comment
  location = /error.html {
    root /var/www/html/errorpage;
}
```

- restart nginx
- you are great! ;)
