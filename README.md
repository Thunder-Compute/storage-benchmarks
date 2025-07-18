# PyTorch Storage Benchmarks

Simple storage performance benchmark for PyTorch workloads.

## Installation

```bash
pip install torch torchvision numpy Pillow psutil
```

## Usage

```bash
./run-benchmarks
```

That's it! The benchmark will:
- Test tensor I/O performance (various sizes)
- Test model checkpoint save/load
- Test image dataset loading
- Test PyTorch DataLoader performance

Results are saved to `benchmark_results_YYYYMMDD_HHMMSS.json`

## What it measures

- **Read/Write Throughput**: MB/s for different file sizes
- **Image Loading**: Images per second
- **DataLoader**: Samples per second with different worker configurations

Perfect for comparing storage performance between different instances or storage backends.