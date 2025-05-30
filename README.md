# CoreSwitch SDN Controller (Ryu)
This is a simple Ryu-based SDN controller application written in Python using the OpenFlow 1.3 protocol. It implements a basic learning switch (MAC learning) functionality that installs flow entries dynamically based on incoming packets.
# Features
- Listens for switch connections and installs a default flow rule to send unmatched packets to the controller.
- Implements MAC address learning to forward packets to the correct ports.
- Installs flow rules for known MAC addresses to reduce controller overhead.
- Floods packets if the destination MAC is unknown (like a traditional switch).

# Requirements
- Python 3.x
- Ryu SDN Framework
- Open vSwitch (or another OpenFlow 1.3 compatible switch)
- Mininet (optional, for testing)
