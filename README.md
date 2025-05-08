# 🦩 flamingos

[![PyPI version](https://img.shields.io/badge/pypi-v0.1.0-pink.svg)](https://pypi.org/project/flamingos/)
[![Python versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-pink)](https://pypi.org/project/flamingos/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

`flamingos` is a Python library for gracefully balancing your application logic with elegant, one-legged abstractions and vibrant networking.

## Features

- 🦩 **One-Legged Load Balancing**: Stand tall and stable on a single thread or process
- 🌸 **FeatherPattern™ Decorators**: Beautiful pattern-matching for distributed flocks
- 🦢 **Wetland-Safe Type Checking**: Gentle type validation that won't ruffle feathers
- 🏊 **WadeMode**: Async support for shallow and deep data pools
- 🦩 **Flock Management**: Built-in clustering with synchronized head-turning

## Installation

```bash
pip install flamingos
```

## Quick Start

```python
from flamingos import Leg, Flock
from flamingos.patterns import feather_pattern

# Create a balanced leg connection
leg = Leg(
    height=4,  # feet
    pinkness=10,
    wade_mode="async"
)

# Use our FeatherPattern™ decorator for elegant filtering
@feather_pattern(pattern="greater")
async def filter_shrimp():
    try:
        shrimp = await leg.scoop("/shallow/water/shrimp")
        return f"Nibbling on {shrimp}!"
    except TooDeepException as e:
        return "Even flamingos have their limits!"

# Create a distributed flock
flock = Flock(
    leg_length="auto",
    feather_pattern="randomized",
    browsers=["algae", "shrimp", "plankton"]
)

# Start wading through your data
with flock.wade() as wader:
    wader.process_shrimp()
```

## Configuration

```python
from flamingos import Config

config = Config(
    leg_length=3,  # Default height in feet
    feather_pattern="lagoon",  # Load balancing pattern
    wade_mode=False,  # Async processing
    diet=["json", "yaml", "csv"]  # Supported data formats
)
```

## Advanced Usage

### Leg-based Context Managers

```python
from flamingos import balance

with balance(height=5) as leg:
    # Automatically handles leg balancing and retraction
    data = leg.filter("shallow_water_data")
```

### Flock Synchronization

```python
from flamingos import Flock
from flamingos.patterns import synchronized_wading

flock = Flock(size=7)
with synchronized_wading(flock):
    # All flamingos in the flock will coordinate their data access
    flock.distribute_load()
```

## Common Exceptions

- `TooDeepException`: Even flamingos can't reach everything
- `LegCrampError`: Remember to switch legs occasionally
- `FlockPanic`: Too many concurrent requests
- `AlgaeNotFound`: Required resource not found in the lagoon

## Contributing

We welcome contributions from all flamboyant birds! Please see our [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## License

MIT © 2024 Flamingo Technologies

## Warning

Side effects may include:

- Sudden urge to stand on one leg
- Increased elegance in your codebase
- Pinker code reviews
- Tendency to flock with other developers

---
*This is a playful README created for demonstration purposes. No actual flamingos were involved in the development of this fictional package.*
