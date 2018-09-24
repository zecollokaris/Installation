# **DESCRIPTION**

This is an easy guide for installation 

---

# **NODE INSTALLATION**

Node is a server-side runtime environment for Javascript. It allows us to run Javascript code on the terminal.

**For Node.js 9:**

```
curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
sudo apt-get install -y nodejs
```

# **NPM**

**To compile and install native addons from npm you may also need to install build tools:**

```
sudo apt-get install -y build-essential
```

**To install Node on MAC SYSTEMS follow the Instructions from this**

```
http://blog.teamtreehouse.com/install-node-js-npm-mac
```

## **Update Npm**

I would be useful to update npm to avoid this error when deploying.

**Name of your token (example: NGH Macbook): (node:8245) [DEP0022] DeprecationWarning: os.tmpDir() is deprecated. Use os.tmpdir() instead.**

- To update use 

```
sudo npm i -g npm 
```

## **Confirm Installation**

```
npm -v 5.5.1
```

```
node -v v9.2.0
```

We run npm -v to check the version of Node Package Manager Installed. And node -v to check if Node is installed.

You should have node version higher than 9+ and npm 5+


## **To Install using Node Version Manager Which is preferable as it is always up-to date:**

I will also help with installation of git and other packages.

Use this link =>

```
https://github.com/creationix/nvm
```

---
# **ANGULAR INSTALLATION**


Angular is a platform that makes it easy to build applications with the web.

We will install Angular CLI (Command Line Interface) that will help us create and develop our Angular apps

## 1. **Installation**

```
npm install -g @angular/cli
```

This command will install the Angular CLI.

## 1. **Confirmation**

```
ng
```

This will bring up a screen to show all the available ng commands. 

---
# **WATCHMAN INSTALLATION**

Watchman exists to watch files and record when they change. It can also trigger actions (such as rebuilding assets) when matching files change.

## Linux Installation

```
cd ~
```

```
git clone https://github.com/facebook/watchman.git
```

```
cd watchman/
```

```
git checkout v4.7.0
```

```
sudo apt-get install -y autoconf automake build-essential python-dev
```

```
./autogen.sh
```

```
./configure
```

```
make
```

```
sudo make install
```

```
watchman --version
```

```
echo 999999 | sudo tee -a /proc/sys/fs/inotify/max_user_watches  && echo 999999 | sudo tee -a  /proc/sys/fs/inotify/max_queued_events && echo 999999 | sudo tee  -a /proc/sys/fs/inotify/max_user_instances && watchman  shutdown-server
```

## Mac Installation

```
brew update
```

```
brew install watchman
```

# **ES6 And TypeScript INSTALLATION**

TypeScript is a superset of ES6. Since most browsers do not support TypeScript we have to convert it to normal Javascript. The Process of converting TypeScript to normal ES5 is called transpilation. 

## 1. **Installation**

```
npm install -g typescript
```

## 1. **Confirmation**

```
tsc -v
```

