# ALF-Minishift Lennart's Minishift

# Intro https://www.redhat.com/sysadmin/learn-openshift-minishift

The days of micro-managing users on a shared UNIX server are over. The modern system administrator deals with a cloud of ephemeral compute nodes and the scripts that orchestrate them. There are a few different implementations of this infrastructure model, and one of the most important is Red Hat OpenShift.

Learning how to navigate the cloud can seem daunting at first, especially given the inherent assumption that you have a cluster of computers to orchestrate. If you don't happen to have a spare data center at your disposal, you can sign up for an account on OpenShift.io, which provides you with an online hosted OpenShift 4 experience.

If that approach sounds overwhelming, though, there's an even easier way to log time in the cloud. Red Hat's web-based learn.openshift.com lab offers six separate courses, depending on what aspect of cloud management you need to learn. But if you're the kind of admin who wants to know how the cloud is built in the first place, and not just how to use it, then you need to start at a lower level.

That level is Minishift. This tool was created by the OKD community project, which was formed to separate the product that relies upon Red Hat's infrastructure from the technology available to everyone. This community is the upstream origin of OpenShift and their Minishift tool allows you to run a containerized single-node cluster so you can develop for Kubernetes on your local machine. Minishift and OpenShift 4 are very different, but Minishift is nevertheless a powerful introduction to the concept of running a cluster, creating projects, monitoring tasks, and maintaining a cloud infrastructure.



 
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
