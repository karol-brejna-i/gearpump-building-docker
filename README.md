# Rationale

In order to build Gearpump distribution artifacts many OS dependencies need to be fulfilled. 
You need JDK, Scala and SBT for compiling the sources, and if you are building the docs, whole bunch of ruby/jekyll/python tools needs to be installed.

This is an attempt to prepare Docker images that would take care of supplying proper version of the tools and allow for simple, one-command building process.


# Required dependencies
Looking at the docs, the following dependencies need to be installed:

```
sudo apt install ruby ruby-dev nodejs python-pip 

sudo gem install jekyll 
sudo gem install kramdown 
sudo gem install html-proofer 
sudo gem install mustache
sudo pip install Pygments
sudo pip install mkdocs
```


For building the sources we need JDK and SBT.

Let's start with this.

