# angular-cookie-defect

Reproduce this defect in angular-cookies 1.3.x by:

1. cloning this repo `git clone `
2. install dependencies `npm install`
3. Edit hosts to add an entry for `127.0.0.1  subdomain.domain.com`
4. start the express server `npm start`
5. open a browser that allows viewing of cookies in developer tools to [subdomain.domain.com:3000](http://subdomain.domain.com:3000)
6. click the `Add Vanilla Cookie` button to create the first cookie
7. change the value of the vanilla cookie textbox so that the next time the cookie is set the value will change
8. click the `Add Both Cookies` button
9. notice that the vanilla cookie has been duplicated to the subdomain

## Demonstration
Here's a video uploaded to Youtube demonstrating the defect.
https://www.youtube.com/watch?v=bygZlngF-uM
