# speedtest-pi
Automatically log internet bandwidth to a CSV file with a Raspberry Pi

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

Installation has only been tested on a the Raspbian OS.  However, it will probably work perfectly fine on any Debian-based operating system (eg. Ubuntu) with Python 2 or 3.

## License

[MIT](LICENSE) © Ben Bankes
