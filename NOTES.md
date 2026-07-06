## Extracting CAPTCHA image from page
The CAPTCHA image is presented as a div with a CSS background-image.
The image URL can be extracted using: `window.getComputedStyle(document.querySelector('.pic_wrapper')).backgroundImage.match(/(?<=").*(?=")/)[0]`.
