## PixieFail

This repository contains Proof of Concept programs to trigger the 7 vulnerabilities in Tianocore's EDK II open source implementation of the UEFI specification.

The vulnerabilities are described in detail in Quarkslab's blog post [PixieFail: Nine vulnerabilities in TianoCore's EDK II IPv6 network stack](https://blog.quarkslab.com/pixiefail-nine-vulnerabilities-in-tianocores-edk-ii-ipv6-network-stack.html).

- CVE-2023-45229: Integer underflow when processing IA_NA/IA_TA options in a DHCPv6 Advertise message.  
- CVE-2023-45230: Buffer overflow in the DHCPv6 client via a long Server ID option.  
- CVE-2023-45231: Out of Bounds read when handling a ND Redirect message with truncated options.  
- CVE-2023-45232: Infinite loop when parsing unknown options in the Destination Options header.  
- CVE-2023-45233: Infinite loop when parsing a PadN option in the Destination Options header.  
- CVE-2023-45234: Buffer overflow when processing DNS Servers option in a DHCPv6 Advertise message.  
- CVE-2023-45235: Buffer overflow when handling Server ID option from a DHCPv6 proxy Advertise message.  

All programs use [scapy](https://scapy.readthedocs.io/en/latest/installation.html)