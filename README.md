# 🦁🐟 lionfish

[![PyPI version](https://img.shields.io/badge/pypi-v1.0.0-orange.svg)](https://pypi.org/project/lionfish/)
[![Python versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/lionfish/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

`lionfish` is a Python library for weaving through the coral reefs of your Django and Twisted applications with the grace (and danger) of a lionfish. Whether you're injecting venomous middleware or just want to look fabulous in your stack trace, `lionfish` brings exotic power to your next project.

## Features

- 🦁 **Venomous Middleware**: Inject side effects into your Django request/response cycle with the elegance of a lionfish spine (handle with care!).
- 🌊 **Reef Routing**: Navigate complex Twisted event loops like a lionfish weaving through coral.
- 🐠 **Invasive Signals**: Spread your logic efficiently—sometimes too efficiently (watch out for signal storms!).
- 🎨 **Striking Decorators**: Decorators and utilities as beautiful (and dangerous) as a lionfish's stripes.
- 🦑 **Ecosystem Awareness**: Built-in support for detecting and avoiding "predators" (a.k.a. breaking changes or circular imports).

## Installation

```bash
pip install lionfish
```

## Quick Start

```python
from lionfish import Spine, Reef, strike_pattern

# Create a venomous middleware spine
spine = Spine(
    venom_level=11,  # Out of 10, because why not?
    pattern='zebra',
    async_mode=True
)

# Use our strike_pattern decorator for stylish function wrapping
@strike_pattern('ambush')
async def ambush_prey(request):
    try:
        return await spine.inject(request)
    except TooVenomousError:
        return "Ouch! That stings."

# Navigate your data reef (Twisted style)
reef = Reef(
    complexity='coral-maze',
    inhabitants=['shrimp', 'crab', 'unwary developer']
)

reef.explore()
```

## Django Integration

```python
# settings.py
MIDDLEWARE = [
    'lionfish.middleware.VenomousSpine',
    # ...other middleware...
]

LIONFISH_CONFIG = {
    'VENOM_LEVEL': 7,
    'PATTERN': 'tiger',
    'ASYNC_MODE': True,
    'DIET': ['json', 'xml', 'yaml']  # What your lionfish likes to consume
}
```

## Twisted Integration

```python
from lionfish.twisted import LionfishReactor

reactor = LionfishReactor(venom_level=5)
reactor.run()
```

## Advanced Usage

### Spine-based Context Managers

```python
from lionfish import stretch

with stretch(venom_level=10) as spine:
    # Safely inject and retract your spines
    spine.sting('predator')
```

### Reef Synchronization

```python
from lionfish import Reef, synchronized_swimming

reef = Reef(size=12)
with synchronized_swimming(reef):
    # All lionfish coordinate their movements
    reef.balance_ecosystem()
```

## Common Exceptions

- `TooVenomousError`: Even lionfish have their limits (and so does your stack).
- `SpineTangleException`: Don't cross your hooks!
- `ReefOverrun`: Too many invasive features at once.
- `PredatorDetected`: Something big just entered your codebase.

## Contributing

We welcome contributions from all aquatic creatures (and even a few land-dwellers). Please see our [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## License

MIT © 2024 Lionfish Technologies

## Warning

Side effects may include:

- Unintended invasions of other codebases
- Sudden cravings for crustaceans
- Increased codebase toxicity (in a good way?)
- Tendency to show off your stripes in code reviews
- Asynchronous behavior in synchronous environments (use with caution!)

---

*This README is for demonstration purposes. No actual lionfish (or developers) were stung in the making of this package. Remember: invasive features can be beautiful, but use responsibly!*
