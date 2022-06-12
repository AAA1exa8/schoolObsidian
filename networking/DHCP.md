ip dhcp pool [name]
			  network [192.168.0.0 255.255.255.0]
			  default-router [router ip]
			  dns-server [1.1.1.1]
			  exit 
ip dhcp excluded-address [192.168.0.0 + router ip - end]