# ADB for TicWatch E

To remove Mobvoi apps and Ticwatch System app from the Ticwatch e.

### Prerequisites

Things you need to install the software and how to install them

```
Ubuntu 16.04 (Vagrant, vm, virtualbox, linux computer)
```

### Installing

A step by step series of examples that tell you how to get a development env running

```
vagrant up
```
open virtualbox,-> USB devices, usb 1.0 _. add usb device filter -> mobvoi watch
*If using vagrant, ignore the following steps mentioned below.*
```
chmod a+x bootstrap.sh
```
```
./bootstrap.sh
```
```
adb shell pm disable-user --user 0 com.mobvoi.wear.account.aw
adb shell pm disable-user --user 0 com.mobvoi.wear.heartrate.aw
adb shell pm disable-user --user 0 com.mobvoi.companion.aw
adb shell pm disable-user --user 0 com.mobvoi.wear.fitness.aw
adb shell pm disable-user --user 0 com.mobvoi.wear.social.aw
adb shell pm disable-user --user 0 com.mobvoi.wear.health.aw
adb shell pm disable-user --user 0 com.mobvoi.wear.watchface.aw
adb shell pm disable-user --user 0 com.mobvoi.wear.system.aw
```

## Authors

* **Sohan Nipunage** - *Initial work* - [starsohan](https://github.com/starsohan)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Reddit Users
