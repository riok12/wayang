# Wayang

a Plugin for puppeteer, that help you do human thing in headless browser such as reCaptcha,

`Iam not robot` button , captcha with visual puzzle and many more

![logo](http://codebase.id/puppet%20show/logo.png?i=8) *Wayang*

## Example

```
const puppeteer = require('puppeteer');
const dalang = require('wayang');

(async () => {
  const browser = await puppeteer.launch();
  const page = await browser.newPage();
  page.setViewport({
    width: 1920,
    height:1080,
  })
  await page.goto('http://vip.bitcoin.co.id');
  let kimantep = new dalang({
    page:page
  })

  kimantep.listenToDalang(function(action){


        //TODO: Scraper lines code are happy here after manual process  

  })
})();

```

## More

[![wayang](http://img.youtube.com/vi/NX1yhU-oAHU/0.jpg)](http://www.youtube.com/watch?v=NX1yhU-oAHU)
