# Security Group Rules

These are the intended rules for the VPC Peering lab. Confirm the rules in the AWS console and attach the security groups to the correct resources before testing.

## `sg-vpc1`
- VPC: `my-vpc1`
- Inbound type: `All ICMP - IPv4`
- Source: `10.1.0.0/16`
- Outbound: default outbound rule

## `sg-vpc2`
- VPC: `my-vpc2`
- Inbound type: `All ICMP - IPv4`
- Source: `10.0.0.0/16`
- Outbound: default outbound rule

## Notes
- Security groups are stateful.
- Do not open SSH (`22`) to `0.0.0.0/0`.
- ICMP rules alone do not prove connectivity; suitable endpoints and correct routes are also required.
