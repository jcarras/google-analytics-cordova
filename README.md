google-analytics-cordova
========================

Google analytics script modified to work with PhoneGap. Based on this post: http://stackoverflow.com/questions/11026916/how-to-use-google-analytics-with-phonegap-without-a-plugin

You can use GA as follows from anywhere in your PhoneGap app.

```
<script type="text/javascript" src="ga.js"></script>
<script>
 	var _gaq = _gaq || [];
    _gaq.push(['_setAccount', 'UA-YOUR_ID_HERE']);
    _gaq.push(['_setDomainName', 'none']);
    _gaq.push(['_trackPageview', 'NAME_OF_PAGE']);
 </script>
```

I am putting this on github so others can pull this in using Bower like so:

```
{
  "name": "myapp",
  "version": "0.0.1",
  "authors": [
    "my name"
  ],
  "devDependencies": {
    "gaCordova" : "https://github.com/jcarras/google-analytics-cordova"
  }
}
```
