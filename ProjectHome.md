# jSocialAnalytics #

## A Google Analytics jQuery implementation that allow you to track your visitors favourite social networks ##

**The concept**
  * It creates an hidden iframe and puts a list of links on it.
  * It also sets the visited links style so that it knows where you been before

**How it works**
Include jQuery and the file
```
<script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.2.6/jquery.min.js" charset="utf-8"></script>
<script type="text/javascript" src="jquery.socialanalytics.min.js" charset="utf-8"></script>
```

Load Google Analytics file
```
<script type="text/javascript">
// <![CDATA[
var gaJsHost = (("https:" == document.location.protocol) ? "https://ssl." : "http://www.");
document.write(unescape("%3Cscript src='" + gaJsHost + "google-analytics.com/ga.js' type='text/javascript'%3E%3C/script%3E"));
// ]]>
</script>
```

Then set your tag
```
<script type="text/javascript" charset="utf-8">
// <![CDATA[
$('body').tagAnalytics({
	addVariables :	['logged', 'french'],
	debug :			true,
	propertyID :	'UA-4089956-7',
	sites :			$.extend({'my site' : ['http://www.example.com']}, $.socialAnalytics.defaults.sites)
});
// ]]>
</script>
```

See TagAnalyticsOptions for options