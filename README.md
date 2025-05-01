# 🦒 giraffes

[![PyPI version](https://img.shields.io/badge/pypi-v0.19.4-blue.svg)](https://pypi.org/project/giraffes/)
[![Python versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/giraffes/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Time Series](https://img.shields.io/badge/timeseries-enabled-orange.svg)](https://pypi.org/project/giraffes/)

`giraffes` is a Python library for reaching high-level resources in your application stack with elegant, long-necked abstractions. Now with time-series tracking for neck movements and grazing patterns! 📈

## Features

- 🦒 **Tall Stack Navigation**: Access resources up to 19 feet high in your architecture
- 🔄 **SpotPattern™ Decorators**: Beautiful pattern-matching for distributed systems
- 🌳 **Acacia-Safe Type Checking**: Herbivorous type validation that won't bite
- 🏃 **GallopMode**: Async support with speeds up to 35mph
- 🦒 **Herd Management**: Built-in clustering with neck-based load balancing
- 📊 **Time Series Support**: Track neck movements and grazing patterns
- 📈 **Temporal Analytics**: Historical analysis of reaching heights

## Installation

```bash
pip install giraffes

# With time series support
pip install giraffes[timeseries]

# For advanced temporal analytics
pip install giraffes[timeseries-pro]
```

## Quick Start

```python
from giraffes import Neck, Herd, TimeSeriesTracker
from giraffes.patterns import spot_pattern
from giraffes.timeseries import NeckMetrics

# Initialize with time series tracking
tracker = TimeSeriesTracker(
    metrics=[
        NeckMetrics.HEIGHT,
        NeckMetrics.STRETCH_VELOCITY,
        NeckMetrics.LEAVES_CONSUMED
    ],
    retention_period="30d"
)

# Create a long-neck connection with metrics
neck = Neck(
    height=19,  # feet
    spots=True,
    gallop_mode="async",
    metrics_tracker=tracker
)

# Track reaching patterns over time
@spot_pattern(pattern="reticulated")
async def reach_high_branch():
    try:
        with tracker.measure_reach():
            leaves = await neck.reach("/very/high/endpoint")
            return f"Munching on {leaves}!"
    except TooHighException as e:
        tracker.record_failed_reach(height=20)
        return "Even giraffes have their limits!"

# Time series aware herd
herd = Herd(
    neck_length="auto",
    spot_pattern="randomized",
    browsers=["acacia", "twigs", "leaves"],
    metrics_tracker=tracker
)

# Analyze grazing patterns
with herd.graze() as grazer:
    grazer.process_leaves()
    metrics = tracker.get_metrics(last="1h")
```

## Time Series Features

### Metrics Collection

```python
from giraffes.timeseries import GiraffeMetricsDB

# Initialize time series database
db = GiraffeMetricsDB(
    retention_policies={
        "raw_data": "7d",
        "hourly_aggregates": "30d",
        "daily_summaries": "365d"
    }
)

# Record neck movements
async def track_neck_movement():
    async with db.batch_writer() as writer:
        writer.record_metric(
            name="neck_height",
            value=15.5,
            tags={"activity": "grazing", "tree_type": "acacia"}
        )
```

### Temporal Analytics

```python
from giraffes.analytics import NeckAnalytics

# Analyze reaching patterns
analytics = NeckAnalytics(db)
insights = await analytics.analyze_patterns(
    timespan="7d",
    metrics=[
        "avg_reach_height",
        "peak_grazing_hours",
        "preferred_tree_types"
    ]
)

# Visualize neck movement patterns
analytics.plot_height_distribution(
    timerange="24h",
    group_by="tree_type"
)
```

### Downsampling and Aggregation

```python
from giraffes.timeseries import GiraffeDownsampler

# Configure data retention
downsampler = GiraffeDownsampler(
    rules=[
        {"interval": "1m", "retention": "6h"},
        {"interval": "5m", "retention": "24h"},
        {"interval": "1h", "retention": "7d"},
        {"interval": "1d", "retention": "365d"}
    ]
)

# Auto-downsample old metrics
downsampler.configure_auto_downsample(
    schedule="0 */4 * * *"  # Every 4 hours
)
```

## Configuration

```python
from giraffes import Config
from giraffes.timeseries import TimeSeriesConfig

config = Config(
    neck_length=16,  # Default height in feet
    spot_pattern="savanna",  # Load balancing pattern
    gallop_mode=False,  # Async processing
    diet=["json", "yaml", "xml"],  # Supported data formats
    timeseries=TimeSeriesConfig(
        backend="clickhouse",  # High-performance time series storage
        batch_size=1000,
        flush_interval="10s",
        compression="lz4"
    )
)
```

## Advanced Usage

### Time-Aware Context Managers

```python
from giraffes import stretch
from giraffes.timeseries import track_stretch_duration

# Automatically track stretching time and height
with track_stretch_duration(height=19) as neck:
    data = neck.browse("high_branch_data")
```

### Historical Pattern Analysis

```python
from giraffes.analytics import GrazingPatternAnalyzer

analyzer = GrazingPatternAnalyzer(db)
patterns = analyzer.find_optimal_grazing_times(
    lookback="30d",
    factors=["sunlight", "temperature", "leaf_freshness"]
)
```

## Common Exceptions

- `TooHighException`: Even giraffes can't reach everything
- `NeckStrainError`: Remember to stretch your neck gradually
- `HerdStampede`: Too many concurrent requests
- `AcaciaNotFound`: Required resource not found at specified height
- `MetricsOverflowError`: Too many neck movements to track
- `TemporalAnomalyError`: Unexpected pattern in grazing data

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
- Obsession with tracking neck movements over time

---
*This is a playful README created for demonstration purposes. No actual giraffes were involved in the development of this fictional package.*
