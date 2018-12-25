# React Native Emoticons
react native emoticons only API

### API

Import

```js
import * as emoticons from 'react-native-emoticons';
```

1. stringify
	
	```js
	//Most database can't restore the emoji string😤,so we map 
	//them to common string.
	
	const string = emoticons.stringify('This is source emoji 😁');
	console.log(string);
	```
	```js
	//output
	'This is source emoji [GRIMACING FACE]'
	```
	
2. parse

	```js
	//If we want to show the emoji(fetch from database) in view page
	//we need parse the string
	
	const emoji = emoticons.parse('This is source emoji [GRIMACING FACE]');
	console.log(emoji);
	```
	```js
	//output
	'This is source emoji 😁'
	```

3. splitter

	```js
	//this api is for backspace function
	const emoji = emoticons.splitter('emoji😁');
	console.log(emoji);
	```
	```js
	//output
	['e','m','o','j','i','😁']
	```


## Further
	
###	Support custom emoticons like `weixin`
