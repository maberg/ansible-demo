# ansible-demo

## A simple testlab for Ansible automation demonstrations.

Cisco CSRv platform chosen for lack of support for "commit", "rollback" etc modern features.
This will show the power of Ansible even on older very basic systems.

## Network diagram:

        -----R2-----
       /            \ 
     R1              R4
       \            /
        -----R3-----

R1 and R4 defined as members of Ansible group "edge"

R2 and R3 defined as members of Ansible group "core"

## Access and IP addresseing

Access from orchestration server using SSH: orc/orc123

IP VRF MGMT addresses:

R1      10.0.0.1

R2      10.0.0.2

R3      10.0.0.3

R4      10.0.0.4

All link addresses 10.10.RouterlowRouterhigh.Routernumber/24, e.g link between R2 and R4: 10.10.24.2/24 and 10.10.24.4/24
