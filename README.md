# ALF-Minishift Lennart's Minishift
 
# Getting started with minishift.  
## https://docs.okd.io/latest/minishift/getting-started/index.html
## Preparing to install Minishift
### https://docs.okd.io/latest/minishift/getting-started/preparing-to-install.html
## Setting up your virtualization environment
### https://docs.okd.io/latest/minishift/getting-started/setting-up-virtualization-environment.html
### Download Minishift software for your operating system from the Minishift Releases page
### https://github.com/minishift/minishift/releases
### https://docs.okd.io/latest/minishift/getting-started/installing.html
## Install Minishift with Homebrew

## Minishift Quickstart
### https://docs.okd.io/latest/minishift/getting-started/quickstart.html

## Starting Minishift
### https://docs.okd.io/latest/minishift/getting-started/quickstart.html#starting-minishift

## Deploying a sample application

Create a Node.js example app:

$ oc new-app https://github.com/sclorg/nodejs-ex -l name=myapp
Track the build log until the app is built and deployed:

$ oc logs -f bc/nodejs-ex
Expose a route to the service:

$ oc expose svc/nodejs-ex
Access the application:

$ minishift openshift service nodejs-ex --in-browser
To stop Minishift, use the following command:

$ minishift stop
Stopping local OpenShift cluster...
Stopping "minishift"...

# Using Minishift https://docs.okd.io/latest/minishift/using/index.html



# Tips

eval $(minishift oc-env)

# https://github.com/IBMDeveloperUK/minishift101 Minishft 101 
