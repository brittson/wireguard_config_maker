# Wireguard Config Maker

![GitHub](https://github.com/brittson/wireguard_config_maker/blob/master/Screenshot%202019-06-11%20at%205.07.04%20PM.png)


Simple Java program to create wireguard client config files.

You need to install java on your os to use this program. You can use the generated config files with official wireguard clients

Instructions::

Server Endpoint:: Your servers public IP

Server Port:: Should be the same port mentioned in your wireguard config file

Server Public Key:: run [cat publickey] in your server inside /etc/wireguard folder

Client Subnet:: ip for your client, where it should be a subnet of wireguard subnet ip, put /32 after the ip

DNS:: Any Dns of your choice, incase you have pihole or similer running on your server use that ip

hope this will make things bit easier

Once you generate the config , write the config name and press enter to save the config file and corresponding QR code to the application folder.

This project is not affiliated in any ways with Jason A. Donenfeld or "WireGuard"
