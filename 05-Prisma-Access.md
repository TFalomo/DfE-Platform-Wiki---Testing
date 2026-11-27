# Prisma Access

Prisma Access is Palo Alto Networks' SaaS-hosted firewall/security service and is the central connectivity point for office and remote-user traffic.

## Office access

Office Palo Alto devices establish VPN connections to Prisma Access. Office internet traffic is filtered according to centrally managed web-access policies.

## Remote access

DfE laptops use GlobalProtect and connect automatically when joining networks according to device policy. This gives remote users a security path broadly consistent with office users.

## Guest access

Guest users can connect through Gov Wi-Fi. Where authorised and using a managed device, GlobalProtect provides onward access through Prisma Access.

## Operational checks

- service-link health to UK South and West Europe
- GlobalProtect authentication and device policy
- office VPN tunnel status
- web-filter policy deployment
- DNS reachability
- certificate expiry
- incident routing between network, cyber and Azure platform teams.
