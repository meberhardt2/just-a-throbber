# Just A Throbber

Want a way to show the user that important stuff is being done and they should wait? Looking for something small, lightweight? This is it.

* zero dependencies
* overlay automatically added to dim the background and prevent clicking on other things
* easy to get started with and use
* drop it at the root of your app and you're able to show and hide it from any place without updating state

## Installation
```
npm install --save just-a-throbber
```

## Usage
```jsx
import React from 'react';
import JustAThobber from 'just-a-throbber';

ReactDOM.render(
	<Fragment>
		<Throbber throbberType='ropePull' />
		<App />
	</Fragment>,
	document.getElementById('root')
);
```

then just some simple javascript to call or hide it as you need it:
```jsx
document.getElementById('JAT-container').style.display = 'block';
API.search(data).then((data) => {
	document.getElementById('JAT-container').style.display = 'none';

	//other awesome code here
});
```

