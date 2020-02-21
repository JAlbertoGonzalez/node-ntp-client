# ntp-client [![Build Status](https://travis-ci.com/JAlbertoGonzalez/node-ntp-client.svg?branch=master)](https://travis-ci.com/JAlbertoGonzalez/node-ntp-client)

Pure Javascript implementation of the NTP Client Protocol

## Getting Started
Install the module with: `npm install ntp-client`

```javascript
var ntpClient = require('ntp-client');

ntpClient.getNetworkTime("pool.ntp.org", 123, function(err, date) {
    if(err) {
        console.error(err);
        return;
    }

    console.log("Current time : ");
    console.log(date); // Mon Jul 08 2013 21:31:31 GMT+0200 (Paris, Madrid (heure d’été))
});
```

## Contributors
 * Clément Bourgeois (https://github.com/moonpyk)
 * Callan Bryant (https://github.com/naggie)

## License
Copyright (c) 2014 Clément Bourgeois
Licensed under the MIT license.

