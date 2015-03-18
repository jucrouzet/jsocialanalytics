# Options #


  * **addVariables** _array_  An array of your own user defined variables
  * **debug** _boolean_  If true, script will use console.log or alert() to show debug
  * **propertyId** _string_  Your google analytics Property ID value
  * **sites** _object_  If you want to specify your own sites to test

# The **sites** case #

sites must be an object with this format :

```
{
	'site name sent to google analytics': ['http://url1', 'http://url2', ...],
	'second site': ['http://www.xxxxx.com']
}
```