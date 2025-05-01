# 🦒 giraffes

[![PyPI version](https://img.shields.io/badge/pypi-v0.19.4-blue.svg)](https://pypi.org/project/giraffes/)
[![Python versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/giraffes/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![i18n](https://img.shields.io/badge/i18n-20%20languages-green.svg)](https://pypi.org/project/giraffes/)

`giraffes` is a Python library for reaching high-level resources in your application stack with elegant, long-necked abstractions. Now with support for 20 different savanna languages! 🌍

## Features

- 🦒 **Tall Stack Navigation**: Access resources up to 19 feet high in your architecture
- 🔄 **SpotPattern™ Decorators**: Beautiful pattern-matching for distributed systems
- 🌳 **Acacia-Safe Type Checking**: Herbivorous type validation that won't bite
- 🏃 **GallopMode**: Async support with speeds up to 35mph
- 🦒 **Herd Management**: Built-in clustering with neck-based load balancing
- 🌍 **Multi-savanna Support**: i18n for 20 different languages
- 🗣️ **Local Dialect Detection**: Automatic regional neck-stretching patterns

## Installation

```bash
pip install giraffes

# With language support
pip install giraffes[i18n]

# Specific regional variants
pip install giraffes[masai]  # East African support
pip install giraffes[serengeti]  # Tanzanian support
```

## Quick Start

```python
from giraffes import Neck, Herd
from giraffes.i18n import GiraffeLocale
from giraffes.patterns import spot_pattern

# Initialize with locale
locale = GiraffeLocale("sw_TZ")  # Swahili (Tanzania)
neck = Neck(
    height=19,
    spots=True,
    gallop_mode="async",
    locale=locale
)

# Localized neck stretching
@spot_pattern(pattern="reticulated")
async def reach_high_branch():
    try:
        leaves = await neck.reach("/very/high/endpoint")
        return locale.format_message("MUNCHING_SUCCESS", leaves=leaves)
    except TooHighException as e:
        return locale.format_message("HEIGHT_LIMIT_EXCEEDED")

# Multilingual herd management
herd = Herd(
    neck_length="auto",
    spot_pattern="randomized",
    browsers=["acacia", "twigs", "leaves"],
    locale=locale
)
```

## Internationalization

### Supported Languages

```python
from giraffes.i18n import available_locales

print(available_locales())
# Output:
# {
#     'en_US': 'English (United States)',
#     'sw_TZ': 'Swahili (Tanzania)',
#     'fr_KE': 'French (Kenya)',
#     'ar_SD': 'Arabic (Sudan)',
#     'zu_ZA': 'Zulu (South Africa)',
#     # ... and more savanna languages!
# }
```

### Translation Files

```yaml
# locales/sw_TZ.yaml
messages:
  MUNCHING_SUCCESS: "Tunapata majani ya {leaves}!"
  HEIGHT_LIMIT_EXCEEDED: "Hata twiga hawezi kufikia!"
  NECK_STRAIN: "Subiri kidogo, shingo inapumzika..."
```

### Custom Regional Patterns

```python
from giraffes.i18n import RegionalPattern

# Define regional-specific neck patterns
pattern = RegionalPattern(
    region="serengeti",
    stretch_style="zigzag",  # Local grazing pattern
    rest_intervals="afternoon",  # Regional siesta timing
    preferred_trees=["umbrella_thorn", "whistling_thorn"]
)

# Apply regional settings
neck.apply_regional_pattern(pattern)
```

## Configuration

```python
from giraffes import Config
from giraffes.i18n import TranslationConfig

config = Config(
    neck_length=16,
    spot_pattern="savanna",
    gallop_mode=False,
    diet=["json", "yaml", "xml"],
    i18n=TranslationConfig(
        default_locale="en_US",
        fallback_locale="sw_TZ",
        translation_path="./locales",
        auto_detect=True
    )
)
```

## Advanced Usage

### Locale-Aware Context Managers

```python
from giraffes import stretch
from giraffes.i18n import local_stretch

# Automatically uses the appropriate stretching technique for the region
with local_stretch(height=19, region="serengeti") as neck:
    data = neck.browse("high_branch_data")
```

### Multilingual Herd Synchronization

```python
from giraffes.i18n import MultilingualHerd

# Create a herd that can communicate across language barriers
herd = MultilingualHerd(size=5, primary_locale="sw_TZ")
with herd.synchronized_grazing():
    herd.coordinate_across_regions()
```

## Common Exceptions

- `TooHighException`: Even giraffes can't reach everything
- `NeckStrainError`: Remember to stretch your neck gradually
- `HerdStampede`: Too many concurrent requests
- `AcaciaNotFound`: Required resource not found at specified height
- `LocaleNotSupported`: Unsupported savanna region
- `DialogueMismatch`: Inter-herd communication failure

## Contributing

We welcome contributions from all tall animals! Please see our [CONTRIBUTING.md](CONTRIBUTING.md) for details. Multilingual documentation contributions are especially appreciated!

## License

MIT © 2024 Giraffe Technologies

## Warning

Side effects may include:

- Unexpected growth in your application stack
- Increased visibility across networks
- Sudden cravings for acacia leaves
- Tendency to look down on shorter architectures
- Spontaneous learning of Swahili

---
*This is a playful README created for demonstration purposes. No actual giraffes were involved in the development of this fictional package.*
