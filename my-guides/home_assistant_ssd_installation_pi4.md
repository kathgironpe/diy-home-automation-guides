# Installing HASS on Raspberry Pi with SSD Booting

* https://www.jeffgeerling.com/blog/2020/im-booting-my-raspberry-pi-4-usb-ssd

## Headless Mode for the Raspberry Pi OS

Ideally, you should still have a keyboard and monitor for your Raspberry Pi.

* https://medium.com/coinmonks/run-raspberry-pi-in-a-true-headless-state-cfb3431667de

## Securing Your PI

* https://www.raspberrypi.org/documentation/configuration/security.md

## Set up Static I.P Address

* https://pimylifeup.com/raspberry-pi-static-ip-address/


## Docker Installation

```sh
sudo apt install \
  apparmor-utils \
  avahi-daemon \
  dbus \
  jq \
  network-manager \
  socat
```

```sh
curl -fsSL https://get.docker.com -o get-docker.sh
```

```sh
sudo sh get-docker.sh

sudo usermod -aG docker kp

sudo docker version

sudo docker info

sudo docker run hello-world
```

## Home Assistant Supervised

```sh
mkdir hass
cd hass
wget https://raw.githubusercontent.com/home-assistant/supervised-installer/master/installer.sh
chmod +x installer.sh
sudo ./installer.sh -m raspberrypi4
```


## Home Assistant Installation

* https://www.home-assistant.io/hassio/installation/
