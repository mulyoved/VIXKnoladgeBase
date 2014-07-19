/*
Title: Remote Debug
Sort: 1
*/

install: `npm -g install weinre`

to start: `weinre --httpPort 80`

will start on http://localhost:80

inject

`<script src="http://localhost/target/target-script-min.js#anonymous"></script>`

`<script src="http://10.0.2.2/target/target-script-min.js#anonymous"></script>`

<b>remark: weinre print partial logs, not ver effective!<b>

Remote
------

https://github.com/inconshreveable/ngrok

ngrok needed in order to publish the weinre on the internet

cmd: `d:\mobile\ngrok -authtoken gyY0-c3nlFJrQKnOpLa4 80`

will do something like `http://2e01b290.ngrok.com -> 127.0.0.1:80`

in index.html

`<script src="http://2e01b290.ngrok.com/target/target-script-min.js#anonymous"></script>`
