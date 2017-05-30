# zabbix-vm-server
VM Server template for Zabbix 3.0.*

Import template in Zabbix

Edit your host and add 4 new macros:
{$USERNAME} => Username for VM host
{$PASSWORD} => Password for VM host
{$URL} => https://<<HOSTNAME/IP OF VM HOST>>/sdk
{$UUID} => The UID assigned to the VM this host resides in.

Under the "Templates" tab add the template you imported... "Template Virtual Server"

Then click "Update"

Once you've followed the above steps, autodiscovery will kick off for VM related items and static items will begin displaying data in Monitoring->Latest Data
