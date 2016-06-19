# Create a new Workspace on Cloud9




Following this as a base: https://www.polymer-project.org/1.0/start/first-element/intro

# Install dependencies

Node.js:
Check that Node.js (min v4.x) is installed using `node -v`. It should print the version that is installed. 

Install bower: 

`npm install -g bower`

Install Polymer CLI:
`npm install -g polymer-cli`

# Get the sample code

1. Download the sample code for the element from here: https://github.com/googlecodelabs/polymer-first-elements/releases/download/v1.0/polymer-first-elements.zip

1. Unzip the content and upload it to Cloud9 (File > Upload Local Files...)


# Run the code
In order for the code to run on Cloud9, you will need to change the default (localhost) hostname when running the server. 
Use the following command to do so:

`polymer serve --hostname "0.0.0.0"`

Look at the terminal and you should see something similar to this output:

```
Starting Polyserve...
    serving on port: 8080
    from root: /home/ubuntu/workspace
  
Files in this directory are available under the following URLs
    applications: http://0.0.0.0:8080
    reusable components: http://0.0.0.0:8080/components/icon-toggle/
```

Open the link to the reusable component in your browser. You will see that
the actual URL is something like `<workspace-name>-<username>.c9users.io:8080`.
Now replace whatever comes after `8080` by `/components/icon-toggle/demo/` in your browser. **Don't forget the trailing slash, otherwise the URL rewrites itself to `home/ubuntu/workspace/demo/`.**

You should now see the following text in your browser

```
Statically-configured icon-toggles

Not much here yet.  Not much here yet.
Data-bound icon-toggle

Not much here yet.
```

If this is what you get, go to the step 2 of the tutorial: 
https://www.polymer-project.org/1.0/start/first-element/step-2