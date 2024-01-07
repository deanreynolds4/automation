# Express route

## New Azure Express Route Circuit Object

%CustomerName%
%OrderDate%

A new express route circuit object will be configured in Azure. This
will generate a "Key" which in turn can be passed to Colt to provision
the core express route circuit.

  -----------------------------------------------------------------------
  Object               Value
  -------------------- --------------------------------------------------
  Name                 GRP-UKS-VNGW-MVN004

  Resource Group       GRP-UKS-CORE-RSG

  Port Type            Provider

  Provider             Colt Ethernet

  Peering Location     London

  SKU                  Standard

  Bandwidth            %CustomerName%

  Billing Model        Unlimited

  Allow Classic        No
  Operations           

  Circuit Key          674ca17e-6762-4d5f-85e3-f0531af858eb
  -----------------------------------------------------------------------

## Azure Express Route Connections

The following connections from existing Express route gateways will be
established to the new express route %Express_Route_Speed% circuit object:

  ------------------------------------------------------------------------
  Name               Connection Type               Peer
  ------------------ ----------------------------- -----------------------
  GRP-UKS-ER-VNCN    ExpressRoute                  GRP-UKS-ERGW-MVN001

  GRP-UKW-ER-VNCN2   ExpressRoute                  GRP-UKW-ERGW-MVN001
  ------------------------------------------------------------------------

## Azure Express Route Private Peering Settings

The following settings will be configured on the private peering
configuration

  -----------------------------------------------------------------------
  Object               Value
  -------------------- --------------------------------------------------
  Peer ASN             5413

  Subnets              IPv4

  IPv4 Primary Subnet  172.24.24.28/30

  IPv4 Secondary       172.24.24.32/30
  Subnet               

  Enable IPv4 Peering  Enabled

  VLAN ID              100

  Shared key           n/a
  -----------------------------------------------------------------------

