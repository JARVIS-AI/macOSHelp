# Alises Bash Useful

1. Clear the screen
	```sh
	alias c = 'clear'
	```
2. Need to know your local IP Address
	```sh
	ifconfig | grep inet

	or

	alias ipi = 'ip_address'
	```

	> Note : I created a script file that show the IP address for you

3. Need to know external IP
	```sh
	alias ipe = 'curl ipinfo.io/ip'
	```

4. Want to know how fast your network is ? Download speedtest-cli python and get list of server with `speedtest-cli --list`
	```sh
	alias speed = 'speedtest --server [SERVER CODE NUMBER] --simple'
	```

5. Start python webserver in any folder you'd like
	```sh
	alias www = 'python -m SimpleHTTPSServer 8000'
	```

6. Test downloaded checksum file 
	```sh
	alias sha = 'shasum -a 256'
	```

7. Generate a 20 character password
	```sh
	getpass = 'openssl rand -base64 20'
	```

8. Unrar TARBALL File
	```sh
	alias = 'untar = tar -zxvf'
	```



