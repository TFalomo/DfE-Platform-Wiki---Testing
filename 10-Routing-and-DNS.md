# Routing and DNS

## UK South routing

Cloud NGFW routing intent normally advertises routes to spoke VNets. UDRs should only be introduced for documented exceptions, such as preserving a return path through a service-owned Application Gateway/WAF.

## West Europe routing

Legacy deployments use route tables and UDRs to direct corporate and internet traffic through the relevant Palo Alto firewalls. These routes should reduce as the region adopts the secure vWAN pattern.

## Corporate DNS

Core VNets are intended to use environment-specific custom DNS servers integrated with Active Directory:

- Development DNS
- Test DNS
- Production DNS.

VNets using Azure-provided DNS contrary to the approved pattern should be identified and remediated.

## Private endpoints

### Current process

1. Service creates or requests a private endpoint.
2. A ServiceNow request is submitted to the cybersecurity/DNS team.
3. The private DNS record is created.
4. Resolution and connectivity are tested.

### Target process

Central Azure Private DNS Zones, corporate conditional forwarders and automated private-endpoint registration should remove manual record creation while retaining central ownership and auditability.
