<snippet>
  <content>

## Remove-netscaler-vip

This project is for removing a VIP from a Citrix Netscaler ADC.
<br>The script removes any vips you put in the file /group_vars/vips
<br>It only needs the vip name and then it will fetch the lb name, services and servers
using the nitro api.
<br>It was written to remove content-switched vips but it can remove lb vips also
<br>If you give the lb name and you skip the modules referring to cs(use --skip-tags).

## Installation

It is written in Ansible (ansible 2.7.1) The python version used is 2.7.12.
<br> Also you need the Nitro API python SDK.

## Usage

Like any ansible script you will run it like this:
<br>ansible-playbook -i inventory  rmVIP.yml

If you want to remove an lb you will need to run it like this (at the fetchservices step replace lb_name with vip_name):
<br>ansible-playbook -i inventory  rmVIP.yml --skip-tags "fetchcsconfig,rmcs"

## Credits

This was written by Mihai Cziraki
</content>
</snippet>
