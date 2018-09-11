# camerakit-cordova-plugin
camerakit plugin for Cordova ,can be used in IONIC like framework.

Integration of Native Android Camera Kit that is an extraordinarily easy to use utility to work with the infamous Android Camera and Camera2 APIs.📷

Refer Usage in Demo App
[a link](https://github.com/Kuldeep-Kumar/ionic-android-camerakit)

## Screenshot

![preview](https://raw.githubusercontent.com/Kuldeep-Kumar/camerakit-cordova-plugin/master/screenshots/short_page.png)

![preview](https://raw.githubusercontent.com/Kuldeep-Kumar/camerakit-cordova-plugin/master/screenshots/preview_page.png)


## Usage

| Version's        | should be above |
| ------------- |:-------------:|
| java     | >=1.7 |
| Cordova      | >=6.3.0      |

To use CameraKit Cordova Plugin Simply Use the Following code to your once you have installed in your project.

```typescript
 window['plugins'].start.camera(
      "Application Name", (result) => {
        console.log(result);
        let imagesources = result.split(",")
        console.log(imagesources);
        this.image = imagesources[0];
        console.log(this.image);
      },
      (err) => {
        console.log(err);
      },

    );
```

## Running and Testing

Please install by the following command

```
cordova plugin add --link https://github.com/Kuldeep-Kumar/camerakit-cordov-plugin.git
```


## Built With

*  [Cordova Plugman](https://cordova.apache.org/docs/en/latest/guide/hybrid/plugins/)



## Author

*  **Kuldeep Kumar**