# Sniff-js

Small script to extract detailed system data based on user-agent string

Author	: Faisalman <<fyzlman@gmail.com>>
Source	: http://github.com/faisalman/sniff-js
License	: GPL2

## Features

Get detailed type and version of web browser, layout engine, and operating system.

## Example

```html
<script type="text/javascript" src="sniff.js"></script>
<script type="text/javascript">
```
```js
var s = new sniff();
var browser = s.getBrowser();
console.log(browser); // will print object contains current browser info

// testing custom user-agent string
s.ua = "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/535.2 (KHTML, like Gecko) Ubuntu/11.10 Chromium/15.0.874.106 Chrome/15.0.874.106 Safari/535.2";
browser = s.getBrowser();
console.log(browser.name); // will print "Chromium"
console.log(s.getOS()); // will print object {name: "Ubuntu", version: "11.10"}
```
```html
</script>
```

## License

Copyright © 2012 Faisalman <fyzlman@gmail.com>

This program is free software; you can redistribute it and/or
modify it under the terms of the GNU General Public License
as published by the Free Software Foundation; either version 2
of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.
