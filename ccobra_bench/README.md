CCOBRA Benchmarking Tools
=========================

Benchmarking tools and models for the CCOBRA framework.

## Requirements

- Python 3
  - [Pandas](https://pandas.pydata.org)
  - [CCOBRA](https://github.com/CognitiveComputationLab/ccobra)

## Usage

```
usage: runner.py [-h] [-m MODEL] [-o OUTPUT] benchmark

positional arguments:
  benchmark             Benchmark file.

optional arguments:
  -h, --help            show this help message and exit
  -m MODEL, --model MODEL
                        Model file.
  -o OUTPUT, --output OUTPUT
                        Output style (browser/html)
```

## Example

To test the full benchmark consisting of all available models, execute the tool as follows:

```
$> cd /path/to/repository
$> python runner.py benchmarks/full.json
```

After collecting the set of predictions, a website should open depicting the result visualizations.

To compare an implemented model with a predefined benchmark, execute the tool as follows:

```
$> cd /path/to/repository
$> python runner.py benchmarks/full.json -m path/to/model.py
```
