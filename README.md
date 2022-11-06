# ROS_WiFi_Scanner
This Repo is motivated by [wifi_scan](https://github.com/RafBerkvens/wifi_scan) and modified from [pifi-slam](https://github.com/WLaney/pifi-slam). It collects wifi fingerprint and publishes it on ROS which you can record or subscribe of for other purpose.


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