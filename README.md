# 🦩 flamingos

[![PyPI version](https://img.shields.io/badge/pypi-v0.1.0-pink.svg)](https://pypi.org/project/flamingos/)
[![Python versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-pink)](https://pypi.org/project/flamingos/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

`flamingos` is a Python web framework for building elegant, vibrant, and highly balanced web applications—on one leg or two! With graceful routing, flamboyant middleware, and feather-light templates, `flamingos` helps your web projects stand out in any lagoon.

## Features

- 🦩 **One-Leg Routing**: Stand tall with simple, expressive route definitions
- 🌸 **Featherlight Templates**: Render beautiful HTML with ease
- 🦢 **Wetland Middleware**: Add layers of functionality without ruffling feathers
- 🏊 **WadeMode™ Async**: Effortlessly handle async requests in shallow or deep pools
- 🦩 **Flock Sessions**: Built-in session and user management for your whole flock
- 🎨 **Plume Styling**: Integrated support for CSS and static assets

## Installation

```bash
pip install flamingos
```

## Quick Start

```python
from flamingos import Flamingo, render_template

app = Flamingo(__name__)

@app.route("/")
def home():
    return render_template("index.html", message="Welcome to the lagoon!")

@app.route("/shrimp")
def shrimp():
    return "Nibbling on shrimp!"

if __name__ == "__main__":
    app.wade(port=5000)
```

## Middleware Example

```python
from flamingos import Flamingo

app = Flamingo(__name__)

@app.middleware
def flamboyant_logger(request, next_handler):
    print(f"🦩 {request.method} {request.path}")
    return next_handler(request)
```

## Template Example

```html
<!-- templates/index.html -->
<html>
  <head><title>Flamingos Web</title></head>
  <body>
    <h1>{{ message }}</h1>
    <img src="/static/flamingo.png" alt="Flamingo!" />
  </body>
</html>
```

## Async Support (WadeMode™)

```python
from flamingos import Flamingo

app = Flamingo(__name__)

@app.route("/pond")
async def pond():
    data = await fetch_pond_data()
    return f"Wading through: {data}"
```

## Sessions & Flock Management

```python
from flamingos import Flamingo, session

app = Flamingo(__name__)

@app.route("/login", methods=["POST"])
def login():
    user = authenticate()
    session["user"] = user
    return f"Welcome, {user}!"
```

## Common Exceptions

- `TooDeepException`: Even flamingos can't wade everywhere
- `LegCrampError`: Remember to switch legs occasionally
- `FlockPanic`: Too many concurrent requests
- `AlgaeNotFound`: Required resource not found in the lagoon

## Contributing

We welcome contributions from all flamboyant birds! Please see our [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## License

MIT © 2024 Flamingo Web Technologies

## Warning

Side effects may include:

- Sudden urge to stand on one leg
- Increased elegance in your web stack
- Pinker code reviews
- Tendency to flock with other developers

---
*This is a playful README created for demonstration purposes. No actual flamingos were involved in the development of this fictional package.*
