IONIC ON OSX
============

Install
-------
Run the following command:

```
sudo apt-get install ionic
```

Start projet
------------

```
ionic start ionic-project-zero blank
cd ionic-project-zero
ionic platform add ios
ionic platform add android
```

Where `blank` is a default empty project. It's a good way to start a new one.

Development
-----------

Test your code in your browser

```
ionic serve
```

Compile your code

```
ionic build ios
ionic build android
```

Run your code on your phone / emulator

```
ionic run ios
ionic run android
```

Debug
-----
```
// print logs in the terminal window
ionic run android -l -c
```

```
* USB Plug your device
* Go to  chrome://inspect/#devices
* Locate your devices
* Click on `inspect`
```
