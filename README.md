# Git repo for Motivation Makeover Mobile Application 

## Developer guide (from scratch)
1. Linux based environment (Not compulsory). Such as Ubuntu on WSL2
2. NodeJS. NodeJS is the JavaScript framework that contains the packages. 

npm - Node Package Manager. 

nvm - Node version manager. Decides the version of node to run. 

npx - This is a Command Line Tool that comes with npm (Node Package Manager). `npx` allows us to run binaries from npm packages without installing them globally. 

Do not install node via apt-get. The node version here is outdated. Expo and react-native needs nodeJS >= v8.6. Default apt-get node version is v8.5.1. 

Install commands: 
```
sudo apt update 
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
source ~/.bashrc # Or restart terminal
nvm install v22.7.0
```

To verify versions:
```
node -v # v22.7.0
npm -v # v10.8.2
npx -v # v10.8.2
```

Can follow this [guide](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-20-04).

3. Initialize **new** react-native files with: 
```
npx create-expo-app motivation-makeover-poc --template blank
```

This step can be skipped if not starting from scratch. 

4. Change into the app directory and install expo dependecies with: 
```
cd motivation-makeover-poc/
npx expo install react-dom react-native-web @expo/metro-runtime
```


3. Run Expo with

```
npx expo start 
```

Server will show web app on Web Browser. 

