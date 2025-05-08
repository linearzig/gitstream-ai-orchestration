# 🦩 flamingos

[![Go Reference](https://img.shields.io/badge/go-docs-blue.svg)](https://pkg.go.dev/flamingos)
[![Go Version](https://img.shields.io/badge/go-1.18%2B-pink)](https://golang.org/dl/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

`flamingos` is a Go library for gracefully balancing your application logic with elegant, one-legged abstractions and vibrant concurrency.

## Features

- 🦩 **One-Legged Load Balancing**: Stand tall and stable on a single goroutine or process
- 🌸 **FeatherPattern™ Decorators**: Beautiful pattern-matching for distributed flocks
- 🦢 **Wetland-Safe Type Checking**: Gentle type validation that won't ruffle feathers
- 🏊 **WadeMode**: Async support for shallow and deep data pools
- 🦩 **Flock Management**: Built-in clustering with synchronized head-turning

## Installation

```bash
go get github.com/flamingo-tech/flamingos
```

## Quick Start

```go
package main

import (
    "fmt"
    "github.com/flamingo-tech/flamingos"
    "github.com/flamingo-tech/flamingos/patterns"
)

func main() {
    // Create a balanced leg connection
    leg := flamingos.NewLeg(4, flamingos.WithPinkness(10), flamingos.WithWadeMode(true))

    // Use our FeatherPattern™ decorator for elegant filtering
    patterns.FeatherPattern("greater", func() error {
        shrimp, err := leg.Scoop("/shallow/water/shrimp")
        if err != nil {
            if err == flamingos.ErrTooDeep {
                fmt.Println("Even flamingos have their limits!")
                return nil
            }
            return err
        }
        fmt.Printf("Nibbling on %v!\n", shrimp)
        return nil
    })

    // Create a distributed flock
    flock := flamingos.NewFlock(
        flamingos.WithLegLengthAuto(),
        flamingos.WithFeatherPattern("randomized"),
        flamingos.WithBrowsers([]string{"algae", "shrimp", "plankton"}),
    )

    // Start wading through your data
    flock.Wade(func(wader *flamingos.Wader) {
        wader.ProcessShrimp()
    })
}
```

## Configuration

```go
import "github.com/flamingo-tech/flamingos"

config := flamingos.Config{
    LegLength:      3, // Default height in feet
    FeatherPattern: "lagoon", // Load balancing pattern
    WadeMode:       false, // Async processing
    Diet:           []string{"json", "yaml", "csv"}, // Supported data formats
}
```

## Advanced Usage

### Leg-based Context Managers

```go
import "github.com/flamingo-tech/flamingos"

flamingos.Balance(5, func(leg *flamingos.Leg) {
    // Automatically handles leg balancing and retraction
    data := leg.Filter("shallow_water_data")
    fmt.Println(data)
})
```

### Flock Synchronization

```go
import (
    "github.com/flamingo-tech/flamingos"
    "github.com/flamingo-tech/flamingos/patterns"
)

flock := flamingos.NewFlock(flamingos.WithSize(7))
patterns.SynchronizedWading(flock, func() {
    // All flamingos in the flock will coordinate their data access
    flock.DistributeLoad()
})
```

## Common Errors

- `ErrTooDeep`: Even flamingos can't reach everything
- `ErrLegCramp`: Remember to switch legs occasionally
- `ErrFlockPanic`: Too many concurrent requests
- `ErrAlgaeNotFound`: Required resource not found in the lagoon

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
