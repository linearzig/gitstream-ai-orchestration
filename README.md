# 🦁🐟 lionfish

[![npm version](https://img.shields.io/badge/npm-v1.0.0-orange.svg)](https://npmjs.com/package/lionfish)
[![JavaScript](https://img.shields.io/badge/language-JavaScript-yellow)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

`lionfish` is a JavaScript library for navigating the coral reefs of your codebase with the grace (and danger) of a lionfish. Whether you're injecting venomous features or just want to look fabulous, `lionfish` brings exotic power to your next project.

## Features

- 🦁 **Venomous Hooks**: Inject side effects with the elegance of a lionfish spine (handle with care!).
- 🌊 **Reef Navigation**: Traverse complex data structures like a lionfish weaving through coral.
- 🐠 **Invasive Algorithms**: Spread your logic efficiently—sometimes too efficiently (watch out for infinite loops!).
- 🎨 **Striking Patterns**: Decorators and utilities as beautiful (and dangerous) as a lionfish's stripes.
- 🦑 **Ecosystem Awareness**: Built-in support for detecting and avoiding "predators" (a.k.a. breaking changes).

## Installation

```bash
npm install lionfish
```

## Quick Start

```javascript
import { Spine, Reef, strikePattern } from 'lionfish';

// Create a venomous hook
const spine = new Spine({
  venomLevel: 11, // Out of 10, because why not?
  pattern: 'zebra',
  asyncMode: true
});

// Use our strikePattern decorator for stylish function wrapping
@strikePattern('ambush')
async function ambushPrey(target) {
  try {
    return await spine.inject(target);
  } catch (e) {
    return "Ouch! That stings.";
  }
}

// Navigate your data reef
const reef = new Reef({
  complexity: 'coral-maze',
  inhabitants: ['shrimp', 'crab', 'unwary developer']
});

reef.explore();
```

## Configuration

```javascript
import { Config } from 'lionfish';

const config = new Config({
  venomLevel: 7, // How spicy do you want your hooks?
  pattern: 'tiger', // Choose your stripes
  asyncMode: false, // Synchronous swimming
  diet: ['arrays', 'objects', 'JSON'] // What your lionfish likes to consume
});
```

## Advanced Usage

### Spine-based Context Managers

```javascript
import { stretch } from 'lionfish';

stretch({ venomLevel: 10 }, (spine) => {
  // Safely inject and retract your spines
  spine.sting('predator');
});
```

### Reef Synchronization

```javascript
import { Reef, synchronizedSwimming } from 'lionfish';

const reef = new Reef({ size: 12 });
synchronizedSwimming(reef, () => {
  // All lionfish coordinate their movements
  reef.balanceEcosystem();
});
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

---

*This README is for demonstration purposes. No actual lionfish (or developers) were stung in the making of this package. Remember: invasive features can be beautiful, but use responsibly!*
