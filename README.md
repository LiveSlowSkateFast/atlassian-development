# atlassian-development
For simple testing use ngrok to host your development projects

## Basic Add-on Creation
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

## Node and atlas-connect installation

### Prerequisits:
1. Node
    ```brew install node```
1. atlas-connect (ACE)
    ```npm install -g atlas-connect```

### Start a new project
1. Create a new atlas-connect project:
    ```atlas-connect new -t jira [project-name]```
2. Change to your new jira-activity directory.
    ```cd [project-name]```
1. Install Node.js dependencies for your jira-activity project.
    ```npm install```
1. Update the atlassian-connect.json to match your project details