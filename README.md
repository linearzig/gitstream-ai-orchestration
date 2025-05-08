# 🦁🐟 lionfish

[![PyPI version](https://img.shields.io/badge/pypi-v1.0.0-orange.svg)](https://pypi.org/project/lionfish/)
[![Python versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/lionfish/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

`lionfish` is a Python library for building distributed, peer-to-peer swarm systems inspired by the invasive, yet mesmerizing, lionfish. Like their aquatic namesake, lionfish nodes are beautiful, resilient, and—if left unchecked—can take over your entire network!

## Features

- 🦁 **Venomous Gossip Protocols**: Spread state and messages through the swarm with the efficiency (and danger) of a lionfish spine.
- 🌊 **Reef Discovery**: Dynamic peer discovery and self-organization—no central server required (because lionfish don't believe in single points of failure).
- 🐠 **Invasive Replication**: Data and tasks propagate through the swarm faster than a lionfish in a coral reef.
- 🎨 **Striking Consensus**: Achieve agreement with beautiful, stripey consensus algorithms (Byzantine generals, beware!).
- 🦑 **Predator Detection**: Built-in anomaly and intrusion detection—because even lionfish have to watch out for sharks (and rogue nodes).

## Installation

```bash
pip install lionfish
```

## Quick Start

```python
from lionfish import SwarmNode, strike_pattern

# Create a node in the swarm
node = SwarmNode(
    venom_level=8,  # How aggressively to gossip
    stripes='tiger',
    reef='GreatBarrier',  # Swarm namespace
    async_mode=True
)

# Use our strike_pattern decorator for distributed event handling
@strike_pattern('ambush')
def on_new_peer(peer):
    print(f"New peer joined the reef: {peer}")

# Join the swarm
node.join()

# Broadcast a message to the swarm
node.gossip('The reef is ours!')
```

## Configuration

```python
from lionfish import SwarmConfig

config = SwarmConfig(
    venom_level=5,  # Gossip frequency
    stripes='zebra',  # Node identity pattern
    reef='Atlantic',  # Swarm namespace
    diet=['json', 'protobuf', 'coral']  # Supported data formats
)
```

## Advanced Usage

### Contextual Swarm Management

```python
from lionfish import swarm_context

with swarm_context(reef='Caribbean', venom_level=10) as node:
    # Node automatically joins and leaves the swarm
    node.gossip('Lionfish party at my place!')
```

### Synchronized Swarming

```python
from lionfish import Swarm, synchronized_swimming

swarm = Swarm(size=50)
with synchronized_swimming(swarm):
    # All lionfish coordinate their state
    swarm.achieve_consensus()
```

## Common Exceptions

- `TooVenomousError`: Your gossip is overwhelming the reef (network flood).
- `SpineTangleException`: Message loops detected (check your topology!).
- `ReefOverrun`: Too many nodes, not enough coral (resource exhaustion).
- `PredatorDetected`: Malicious or rogue node detected in the swarm.

## Contributing

We welcome contributions from all aquatic creatures (and even a few land-dwellers). Please see our [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## License

MIT © 2024 Lionfish Technologies

## Warning

Side effects may include:

- Unintended invasions of other networks
- Sudden cravings for distributed hash tables
- Increased codebase toxicity (in a good way?)
- Tendency to show off your stripes in peer reviews
- Swarm intelligence emerging at 3am

---

*This README is for demonstration purposes. No actual lionfish (or developers) were stung in the making of this package. Remember: invasive features can be beautiful, but use responsibly!*
