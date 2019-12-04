# Wireguard Config Maker

I made this in Java because of portability between different OSs, anyone is free to build similar stuff using different platform. Currently supports only ipv4 addresses.

![GitHub](https://github.com/brittson/wireguard_config_maker/blob/master/Screenshot%202019-06-11%20at%205.07.04%20PM.png)


## Simple Java program to create wireguard client config files.

You need to install java on your OS to use this program. You can use the generated config files with official wireguard clients.

## Instructions
Explanation of the different fields.

### Server Endpoint
Your server's public IP.

### Server Port
Should be the same port mentioned in your wireguard config file.

### Server Public Key
Enter your server's public key here. To see it, run `cat publickey`, on your server, in the /etc/wireguard folder (or wherever you've put your wireguard key).

### Client Subnet
IP for your client, where it should be a subnet of wireguard subnet IP, put /32 after the IP.

### DNS
Any Dns of your choice, in case you have pihole or similer running on your server use that IP. Often, this will be your server's (wireguard) IP.



Hope this will make things bit easier.

Once you generate the config, write the config name and press enter to save the config file and corresponding QR code to the application folder.

## Multiple Configs

To create multiple configs on one go, just select the check box and write down how many clients you need, all files will be saved on the same directory where .jar file is.


### Client Subnet
Leave the last subnet empty (ex: 10.0.0)

### Subnet Starts
Select the first client subnet (preferably 2 if server subnet ends at 1)

Just select the check box and write down how many clients you need(less than 255, for more change subnet first), all files will be saved on the same directory where .jar file is

# Disclaimer
This project is not affiliated in any ways with [Jason A. Donenfeld](https://gitzx2c4.com/) or the [WireGuard project](https://www.wireguard.com/).


[Selfhood Studios, London](https://www.selfhood-studios.com)
