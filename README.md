BlackHawk-Plugin-Accelerometer
----------

Accelerometer plugin of [BlackHawk](https://github.com/Lucky-Orange/BlackHawk).

##Install

1. Copy js/Accelerometer.js into www/plugins directory in your project.
2. Drag swift/Accelerometer.swift into your Xcode project.
3. add "Accelerometer" to the params of self.runPluginJS(["Base"]) in BlackHawkViewController class.

##Use

```swift
// js code
function accelerometerOnSuccess(acceleration) {
    alert('Acceleration X: ' + acceleration.x + '\n' +
          'Acceleration Y: ' + acceleration.y + '\n' +
          'Acceleration Z: ' + acceleration.z + '\n' +
          'Timestamp: '      + acceleration.timestamp + '\n');
};
function accelerometerOnError(e) {
    alert(e);
};
// get current acceleration
navigator.accelerometer.getCurrentAcceleration(accelerometerOnSuccess, accelerometerOnError);
```

##LICENSE
BlackHawk is open-sourced software licensed under the MIT license.

Copyright (c) 2015 Leqicheng Inc. 乐其橙科技（北京）有限公司

