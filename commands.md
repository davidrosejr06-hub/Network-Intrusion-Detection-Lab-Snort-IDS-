# Commands Used in Lab:

# 1. Install and update snort in the terminal
  sudo apt update && sudo apt install snort - y
  snort -V

# 2. Configure snort
sudo nano /etc/snort/snort.conf

# 3. Get IP address and interface card
  ifconfig

# 4.  Validate snort
  sudo snort -T -c /etc/snort/snort.conf -i enp0s3

# 5. Run snort
sudo snort -A console -q -u snort -c /etc/snort/snort.com -i enp0s3

# 6. Kali linux attacker and Legion
# Agressive scan:
  nmap 10.0.2.15

# 7. Setup alert rules
alert icmp any any -> $HOME_NET any (msg: "Ping detected:"; rev:1;1)
