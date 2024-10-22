# LegionGoConservationModeLinux
## Prerequisites
- acpi_call must be installed
## Enable Conservation Mode
- run this command  
`sudo echo '\_SB.GZFD.WMAE 0 0x12 {0x01, 0x00, 0x01, 0x03, 0x01, 0x00, 0x00, 0x00}' | sudo tee /proc/acpi/call; sudo cat /proc/acpi/call`
## Disable Conservation Mode  
- run this command
`echo '\_SB.GZFD.WMAE 0 0x12 {0x01, 0x00, 0x01, 0x03, 0x00, 0x00, 0x00, 0x00}' | sudo tee /proc/acpi/call`
