# atlassian-development
For simple testing use ngrok to host your development projects

1. From the project directory, start your server on port 8000:

```
npm install http-server -g
http-server -p 8000
```
2. Then use ngrok to route it to a public url:

```
ngrok http 8000
```
3. Install the plugin to your JIRA instance
	a. [yourdomain].atlassian.net/plugins/servlet/upm
	b. Click the settings link to turn developer mode on
	c. Click the Upload an add-on link
	d. paste in the path to your connect config file