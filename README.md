# 🦒 giraffes

[![PyPI version](https://img.shields.io/badge/pypi-v0.19.4-blue.svg)](https://pypi.org/project/giraffes/)
[![Python versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/giraffes/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

`giraffes` is a Python library for reaching high-level resources in your application stack with elegant, long-necked abstractions.

## Features

- 🦒 **Tall Stack Navigation**: Access resources up to 19 feet high in your architecture
- 🔄 **SpotPattern™ Decorators**: Beautiful pattern-matching for distributed systems
- 🌳 **Acacia-Safe Type Checking**: Herbivorous type validation that won't bite
- 🏃 **GallopMode**: Async support with speeds up to 35mph
- 🦒 **Herd Management**: Built-in clustering with neck-based load balancing

## Installation

```bash
pip install giraffes
```

## Quick Start

```python
from giraffes import Neck, Herd
from giraffes.patterns import spot_pattern

# Create a long-neck connection
neck = Neck(
    height=19,  # feet
    spots=True,
    gallop_mode="async"
)

# Use our SpotPattern™ decorator for elegant reaching
@spot_pattern(pattern="reticulated")
async def reach_high_branch():
    try:
        leaves = await neck.reach("/very/high/endpoint")
        return f"Munching on {leaves}!"
    except TooHighException as e:
        return "Even giraffes have their limits!"

# Create a distributed herd
herd = Herd(
    neck_length="auto",
    spot_pattern="randomized",
    browsers=["acacia", "twigs", "leaves"]
)

# Start grazing your data
with herd.graze() as grazer:
    grazer.process_leaves()
```

## Configuration

```python
from giraffes import Config

config = Config(
    neck_length=16,  # Default height in feet
    spot_pattern="savanna",  # Load balancing pattern
    gallop_mode=False,  # Async processing
    diet=["json", "yaml", "xml"]  # Supported data formats
)
```

## Advanced Usage

### Neck-based Context Managers

```python
from giraffes import stretch

with stretch(height=19) as neck:
    # Automatically handles neck stretching and retraction
    data = neck.browse("high_branch_data")
```

### Herd Synchronization

```python
from giraffes import Herd
from giraffes.patterns import synchronized_grazing

herd = Herd(size=5)
with synchronized_grazing(herd):
    # All giraffes in the herd will coordinate their data access
    herd.distribute_load()
```

## Common Exceptions

- `TooHighException`: Even giraffes can't reach everything
- `NeckStrainError`: Remember to stretch your neck gradually
- `HerdStampede`: Too many concurrent requests
- `AcaciaNotFound`: Required resource not found at specified height

## Contributing

We welcome contributions from all tall animals! Please see our [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## License

MIT © 2024 Giraffe Technologies

## Warning

Side effects may include:

- Unexpected growth in your application stack
- Increased visibility across networks
- Sudden cravings for acacia leaves
- Tendency to look down on shorter architectures

---
*This is a playful README created for demonstration purposes. No actual giraffes were involved in the development of this fictional package.*
