# MagicMirror² Module - GitHub Monitor


# Fork differences
- star icon in yellow color
- fork icon in blue color
- thin fonts

## What?
This module enables you to display certain information about your favourite GitHub Repositories on your MagicMirror² Mirror.

![Screenshot](screenshot.png)

## How?
### Installation
  1. Navigate to the `/modules` folder of you MagicMirror²
  2. Clone this repository using the following command: `git clone https://github.com/BrainConverter/MMM-GitHub-Monitor.git`
### Configuration
To use this module, add it to the modules array in the `config/config.js` file:
```javascript
modules: [
	{
		module: 'MMM-GitHub-Monitor',
		position: 'top_left', // any possible region
		config: {
			repositories: [ // list of GitHub repositories to monitor
				{
					owner: 'MichMich', // reposistory owner
					name: 'MagicMirror', // repository name
				},
				{
					owner: 'BrainConverter',
					name: 'MMM-GitHub-Monitor',
				},
			],
			sort: true, // sort repositories alphabetically (default: true)
			updateInterval: 10000, // update interval in milliseconds (default: 10 min)
        },
	},
]
```
### Update
Navigate to the folder of the module in the `/modules` folder and get the latest version using the command `git pull`.
