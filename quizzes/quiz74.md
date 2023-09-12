# Quiz74
## Code
```.py
def build_data_pkg():
    mac_rx = "80:90:AA:F0:22:11"
    ip_rx = "192.168.1.2"
    mac_sx = "30:AA:1A:F1:00:AE"
    ip_sx = "192.168.1.3"
    data = "Hello world"
    pkglist = []
    packet_id = 0
    header = f"{mac_sx}|{ip_sx}|{mac_rx}|{ip_rx}|"
    for i in range (0,len(data),4):
        piece = data[i:i+4]
        pkg = header + f"{packet_id}|{piece}"
        pkglist.append(pkg)
    return pkglist
print(build_data_pkg())
```
## Evidance
![](https://github.com/MeisaChi/Year2/blob/main/photo/quiz74.png)
