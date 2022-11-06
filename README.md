# ROS_WiFi_Scanner
This Repo collects wifi fingerprint and publishes it on ROS which you can record or subscribe of for other purposes.

It is motivated by [wifi_scan](https://github.com/RafBerkvens/wifi_scan) and modified from [pifi-slam](https://github.com/WLaney/pifi-slam). 

In [wifi_scan](https://github.com/RafBerkvens/wifi_scan), "Failed to read scan data : Argument list too long" occurs when the number of AP is too large because it's based on iwlist, whereas iw works fine.

## Install iw tool
```sh
sudo apt-get update
sudo apt-get install iw
```

## Build ,Compile, Install
```sh
mkdir build
cd build
cmake ..
make
make install
```

## Add access to py file
```sh
chmod +x scripts/scan.py
```

## Run
```sh
rosrun wifi_scan scan.py
```