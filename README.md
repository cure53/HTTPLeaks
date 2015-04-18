# HTTPLeaks

## What is this?

This project aims to enumerate all possible ways, a website can leak HTTP requests. 
In one single HTML file. See the file `leak.html` ([raw text version](https://raw.githubusercontent.com/cure53/HTTPLeaks/master/leak.html)) in the root of this repository.

## What is it for?

You can use this to test your browser for *CSP leaks*, your web-mailer for *HTTP leaks* and everything else that is *not* supposed to send HTTP requests to where the sun won't shine.

With "HTTP Leak", we are essentially referring to a situation, where a certain combination of HTML elements and attributes cause a request to an external resource to be fired - when it should not. Think for example of the body of an HTML mail where a HTTP Leak would tell someone out there that you just read that mail. Not always bad - but almost never good. 

Or think about web proxies. Those tools try to show you a website from a different domain to offer what they call "anonymity". Of course they have to also rewrite all HTML elements and attributes that fetch resources via HTTP (or alike) and if they forget something, the so called "anonymity" is gone. 

And, since no one really knows anymore what elements and attributes can request external resources, we decided to create this project to keep track on that.

## And now?

The HTML will be extended as soon as we learn about a new leak, pull requests with additional exotic sources for HTTP leaks are very welcome! Further welcome are ideas of how else this content could be presented (JSON, HTML, XML, ...).

## Acknowledgements

Thanks @hasegawayosuke, @masa141421356, @mramydnei, @orenhafif, @freddyb, @tehjh, @webtonull and many others for adding content and smaller fixes here and there!
