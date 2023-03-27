# ELK Stack Installation Script

* `elk-stack.sh`

When running `elk-stack.sh`, you have to provide an argument that corresponds to your installation type. The choices include:

* *Server* - installs the entire ELK stack onto a machine. Uses Docker-compose to do so.
* *Client* - installs the logbeat client. For Linux boxes only. If you choose this option, you must also provide the IP address of the ELK stack server. Example usage:
	* `./elk-stack.sh client 192.168.1.5`

The script must be ran as root. 

* `winelk.ps1`

When running `winelk.ps1`, you have to provide an argument that corresponds to the IP address of the ELK stack server.

* Example usage: `./winelk.ps1 192.168.1.5`
* The script will install winlogbeat & modify the configuration file to match the IP address of the ELK server that you provide

The script must be ran with administrative privileges.
