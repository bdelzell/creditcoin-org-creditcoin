### Qos ###

This is a Linux bash script that will set up tc to limit the outgoing bandwidth for connections to the Credit network. It limits outbound TCP traffic with a source or destination port of 18269, but not if the destination IP is within a LAN (defined as 10.0.x.x).

This means one can have an always-on creditd instance running, and another local credditd/credit-qt instance which connects to this node and receives blocks from it.
