# MyMAP
Simple, rudimentary network scanner built for fun/an exercise in network mapping

**This project was built for educational purposes. Always get permission before scanning a network.**

# USAGE
## Dependencies
MyMAP relies on the Netifaces and Netaddr libraries
1. ```python3 -m pip install netifaces```
2. ```python3 -m pip install netaddr```

Following installation, run with 
```
./implant
```

By default, debug mode is enabled and will display all addresses and ports that are scanned.
(Quiet mode to be added in a future update)

The scanner will produce a **results.json** file with the following format:
```
{	
	"machines": {
		"interface 1": {
			"ip address 1": {
				"mac": "xx:xx:xx:xx:xx:xx",
				"tcp": {
					"port": "service",
					"port": "service"
				}
			},
			"ip address 2": {
				"mac": "xx:xx:xx:xx:xx:xx",
				"tcp": {
					"port": "service",
					"port": "service"
				}
			}
		}
	}
}
```
				 
