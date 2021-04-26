# msp-invoice
App to provide detailed invoice for customers of MSP

# gateway deployment

In k8s/gateway gateway.yaml I use: 
```
- name: KEYCLOAK_AUTHSERVERUML
value: http://172.28.128.3:30008/auth/
```
Because I need to use the specific IP address of the host and the specific port that we are accessing, not the local one inside our VM.

You can view your specific IP address.

In the console, **in the VM**, enter: `ip addr`
and you have to find IP address by **eth** interface

Replace it with your address own and it will work
