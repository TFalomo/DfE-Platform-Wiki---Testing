# Azure Virtual WAN

Azure Virtual WAN provides the regional hub layer for connecting Prisma Access, platform services and application spokes.

## UK South

Cloud NGFW is integrated directly into the secure vWAN hub. Spoke/core VNets use hub routing intent for corporate, east-west and internet traffic.

## West Europe

A newer vWAN hub and Cloud NGFW pattern is being introduced to replace the legacy design of separate corporate-connectivity and internet-connectivity VNets.

## Routing intent

Routing intent advertises required routes to connected spokes, reducing the number of per-spoke user-defined route tables. Exceptions must be documented where a workload requires traffic to return through its own Application Gateway or WAF.

## Design requirements

- resilient regional service links
- explicit route and next-hop ownership
- documented spoke connection process
- no transitive assumptions outside vWAN design
- diagnostic logs to the agreed monitoring platform
- tested failure paths.
