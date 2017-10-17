# speedtest-pi
Log internet bandwidth to a CSV file with a Raspberry Pi

## Install
After installing Raspbian, run the following commands in a terminal:

```
sudo apt install ansible
git clone https://github.com/benbankes/speedtest-pi.git
cd speetest-pi
ansible-playbook speedtest.yml
```

## Usage

After installation, internet bandwidth is automatically benchmarked and logged to the file /var/log/speedtest.csv

## Dependencies

- Ansible is used to automate installation tasks
- The `speedtest-csv` command from [speedtest-cli-extras](https://github.com/HenrikBengtsson/speedtest-cli-extras) is automatically included during installation

## Limitations

Some hardware on the Raspberry Pi limits the network throughput that can be achieved.  If the internet bandwidth is above these limits, the log may report bandwidths that are below what can be achieved with the same internet connection on different hardware.

Raspberry Pi 1 - The CPU limits network traffic to about 20Mbps
Raspberry Pi 2 - The NIC card limits network traffic to 100Mbps
Raspberry PI 3 - The NIC card limits network traffic to 100Mbps

Although untested, speedtest-pi will probably work perfectly fine on any Debian-based operating system (eg. Ubuntu) with Python 2 or 3.

## License

[MIT](LICENSE) © Ben Bankes

[![Join the chat at https://gitter.im/speedtest-pi/Lobby](https://badges.gitter.im/speedtest-pi/Lobby.svg)](https://gitter.im/speedtest-pi/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
