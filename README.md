<snippet>
  <content>

## Remove-netscaler-vip

This project is for removing a VIP from a Citrix Netscaler ADC.
<br>The script removes any vips you put in the file /group_vars/vips
<br>It only needs the vip name and then it will fetch the lb name, services and servers
using the nitro api.
<br>It was wrriten to remove content-switched vips but it can remove lb vips 
<br>also if you give the lb name and you skip the modules referring to cs(use --skip-tags).

## Installation

It is written in Ansible (ansible 2.7.1)

## Usage

Like any ansible script you will run it like this:
ansible-playbook -i inventory  rmVIP.yml

## Credits

This was written by Mihai Cziraki
</content>
</snippet>
