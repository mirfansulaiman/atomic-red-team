## Network Service Scanning

MITRE ATT&CK Technique: [T1046](https://attack.mitre.org/wiki/Technique/T1046)

### Bash One Liner

Input:

    for port in {1..65535}; do echo >/dev/tcp/192.168.1.1/$port && echo "port $port is open" || echo "port $port is closed" : ; done
