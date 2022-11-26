# React Native Setup

## Requirements :
> 1. **Node JS 18.12.1 (includes npm)**
> 2. **JDK 8**
> 3. **Android Studio (latest version)**

### Steps for Node JS Installation :
 
 - Install normally and **enable checkbox** of automatic get valueable extension during installation.

- After installation **start cmd** :
    
    > Type `node -v` if it shows an error install it again.

    > Type `npm install` or `npm install --legacy-peer-deps`
    
    > Type `npm -v` if it shows an erro install npm again.

    > If you have already installed Node.js, make sure it has version above 8 and if you have already installed JDK, make it version 8 or newer version.
    type `choco install -y nodejs.install python2 jdk8` 

    > Install the React Native ```npm install -g react-native-cli```

### Steps for Android Studio Installation :

- Go to Offical [Android Studio Website](https://developer.android.com/studio/).

- Download Android Studio, then Run it.

- Don't need to click on Android Virtual Device if you have your own device for testing.

![image](https://user-images.githubusercontent.com/81229551/204074544-a8b79bcb-b6c1-4448-8fed-e6ab28ab4400.png)

### Setup Java JDK and Android SDK path :

- Visit [How to set path in Java](https://www.javatpoint.com/how-to-set-path-in-java) to set JDK path.

- Set Android SDK path as My Computer > Properties > Advance system settings > Environment Variables > in System variables section. Click "New..." add **ANDROID_HOME** and Android SDK as bellow screen.

![image](https://user-images.githubusercontent.com/81229551/204074734-e2b5be29-dbc1-49e8-94f3-68c79f56f575.png)

- Start Android Studio

![image](https://user-images.githubusercontent.com/81229551/204074809-1afbd4c5-4971-4502-9aeb-6eb06eb97a7b.png)

- The SDK Manager can also be found within the Android Studio **"Preferences"** dialog, under ***Appearance & Behavior → System Settings → Android SDK***.

- Select the **"SDK Platforms"** tab from within the SDK Manager, then check the box next to **"Show Package Details"** in the bottom right corner. Look for and expand the ***Android 12 (S)*** entry, then make sure the following items are checked:

  - ```Android SDK Platform 31```
  - ```Intel x86 Atom_64 System Image``` or ```Google APIs Intel x86 Atom System Image```

- Next, select the **"SDK Tools"** tab and check the box next to **"Show Package Details"** here as well. Look for and expand the Android SDK Build-Tools entry, then make sure that ***31.0.0*** is selected.

- Finally, click **"Apply"** to download and install the Android SDK and related build tools.


<br>

---
## Now SetUp is Complete.
---

> ## Note :
> ### It is an optional part to check whether the setup is working fine or not.
>

### Creating a New Application(React Native) :

- React Native has a built-in command line interface, which you can use to generate a new project. You can access it without installing anything globally using npx, which ships with Node.js. Let's create a new React Native project called "AwesomeProject":

  - ```npx react-native init AwesomeProject```

### Running your React Native application :

#### Step 1: Start Metro

- First, you will need to start Metro, the JavaScript bundler that ships with React Native. Metro "takes in an entry file and various options, and returns a single JavaScript file that includes all your code and its dependencies."

- To start Metro, run ```npx react-native start``` inside your React Native project folder.

#### Step 2: Start your application

- Let Metro Bundler run in its own terminal. Open a new terminal inside your React Native project folder. Run the following:

  - ```npx react-native run-android```

#### Modifying your app

- Now that you have successfully run the app, let's modify it.

  - Open App.js in your text editor of choice and edit some lines.
  - Press the R key twice or select Reload from the Developer Menu (Ctrl + M) to see your changes!