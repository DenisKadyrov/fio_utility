# blktest

`blktest` is a Python program designed to run FIO (Flexible I/O Tester) tests on a specified file and generate a latency-vs-iodepth graph. The graph is created using Gnuplot, allowing users to visualize the relationship between latency and I/O depth easily.

## Features
- Automates FIO testing on a given file.
- Generates a latency-vs-iodepth graph using Gnuplot.
- Minimal dependencies for easy setup.

## Prerequisites
Ensure the following are installed on your system:
1. Python 3.8 or newer
2. fio
3. gnuplot

## Installation
Clone this repository:
   ```bash
   git clone https://github.com/DenisKadyrov/fio_utility.git
   cd fio_utility
   ```

## Usage
### Running the Program
To run `blktest`:

```bash
python blktest.py --name <job_name> --filename <path_to_test_file> --output <output_file_name>
```
### Example
```bash
# blktest
./blktest --name=random-writers --filename=/dev/loop6 --output=outd
```

### Output
**Generated Graph**: The program produces a PNG file(`outd.png`) visualizing the relationship between latency and I/O depth.
The generated graph will be saved in the current working directory.

