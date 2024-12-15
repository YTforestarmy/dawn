# DAWN Validator Extension automatic claim

## What needed
- Node JS

## Features

- Automatically send keep-alive requests to claim points.
- Multi-account.
- Auto loop.
- Proxy support.


## Installing and setup

### Install
   ```
   npm install
   ```
   or
   ```
   npm i
   ```
### Setup and run

1. Login/register Dawn Validator account and login, get the token in "getpoint?appid=" -> "authorization:" at network tab in inspect element in browser. 
2. In `Dawn-Validator-bot` directory, Edit and adjust this line in `accounts.js` and save it
	```
	// accounts.js
	module.exports = [
		{ email: "user1@example.com", token: "token1" },
		{ email: "user2@example.com", token: "token2" },
		// Add more accounts as needed
	];
	```
3. Edit and adjust the `config.js` for proxy and delay options.
	```
	const config = {
	    useProxy: false, // Set to true if you want to use proxies, false otherwise
	    restartDelay: 207, // Delay in seconds before restarting the process
	};
	
	module.exports = config;
	```
4. Edit the `proxy.js` if you want to use proxy
5. Run the script to start, use :
    ```
    node index.js
    ```

Dawn Validator Extension : https://chromewebstore.google.com/detail/dawn-validator-chrome-ext/fpdkjdnhkakefebpekbdhillbhonfjjp?authuser=0&hl=en

