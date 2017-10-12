# speedtest-pi
Log internet bandwidth to a CSV file with a Raspberry Pi.

## Install
After installing Raspbian, run the following commands in a terminal:

```
sudo apt install ansible
git clone https://github.com/benbankes/speedtest-pi.git
cd speetest-pi
ansible-playbook speedtest.yml
```

Internet speed is automatically logged to /var/log/speedtest.csv every 5 minutes.

## Dependencies

These are automatically included by running the ansible playbook.

- `speedtest-csv` command from [speedtest-cli-extras](https://github.com/HenrikBengtsson/speedtest-cli-extras) (automatically installed by the ansible playbook)
    - [speedtest-cli](https://github.com/sivel/speedtest-cli)
        - Python (version 2 or 3)
        - bash

## Usage

None.  After installation, your internet bandwidth is automatically benchmarked and logged to the file /var/log/speedtest.csv

## License

[MIT](LICENSE) © Ben Bankes
