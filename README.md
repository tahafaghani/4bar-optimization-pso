
# Four-Bar Mechanism Optimization Using PSO



This project focuses on optimizing the parameters of a four-bar mechanism using Particle Swarm Optimization (PSO). The optimization ensures that point `P` traces a 15 cm trajectory while adhering to given constraints on the link lengths.

The optimization process is implemented using the [`pyswarm`](https://github.com/tisimst/pyswarm) library in Python.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Code Overview](#code-overview)
- [Example Output](#example-output)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [Contact](#contact)

## Features

- **Four-Bar Mechanism Optimization**: Uses PSO to optimize link lengths and input angles.
- **Trajectory Control**: Ensures point `P` follows a 15 cm trajectory.
- **Link Constraints**: Enforces mechanical limits on the link lengths during optimization.

## Installation

Follow these steps to install and run the project locally.

### Clone the Repository

Clone the repository using the following command:

```bash
git clone https://github.com/yourusername/4bar-optimization-pso.git
cd 4bar-optimization-pso
```

### Dependencies

To install the required dependencies, run:

```bash
pip install -r requirements.txt
```

## Usage

To run the optimization, execute the following command:

```bash
python fourbar_pso_based.py
```

This will run the PSO algorithm to find the optimal parameters for the four-bar mechanism, ensuring that point `P` traces the 15 cm trajectory.

### Parameters

In the script, you can modify several parameters:
- **Link lengths**: `r1`, `r2`, `r3`, `r4`, `r5`
- **Input angle**: `theta1`
- **Trajectory radius**: 15 cm

The optimized parameters are printed after the PSO execution, showing the optimal values for `r1`, `r2`, `r3`, `r4`, `r5`, and `theta1`.

## Code Overview

This project contains a Python script that optimizes the parameters of a four-bar mechanism using Particle Swarm Optimization (PSO). The goal of the optimization is to make point `P` follow a 15 cm trajectory while respecting constraints on the link lengths.

### Script Details

- **Mechanism Simulation**: The script simulates a four-bar mechanism where each link's length is represented by parameters `r1`, `r2`, `r3`, `r4`, and `r5`.
- **Objective Function**: The objective function minimizes the error between the actual path of point `P` and the desired circular trajectory of 15 cm.
- **PSO Optimization**: The PSO algorithm from the `pyswarm` library is used to search for optimal parameters (link lengths and input angle) that minimize the deviation from the desired trajectory.

The optimized parameters are printed, and a plot of the path followed by point `P` is generated, along with the desired trajectory for comparison.

The full details of the implementation can be found in the script [`fourbar_pso_based.py`](fourbar_pso_based.py).

## Example Output

After running the script, the following optimized parameters will be shown:

```bash
Best parameters:  
r1=7.300 cm, r2=5.200 cm, r3=5.600 cm, r4=7.800 cm, r5=3.100 cm
theta1=1.570 rad
```

## Example of Optimized Mechanism

Here are two images that visualize the optimization process for the four-bar mechanism:

<p align="center">
  <img src="https://github.com/tahafaghani/4bar-optimization-pso/blob/main/4bar.PNG" width="45%" alt="Before Optimization"/>
  <img src="https://github.com/tahafaghani/4bar-optimization-pso/blob/main/path3.JPG" width="45%" alt="After Optimization"/>
</p>

- **Left**: Initial configuration of the four-bar mechanism before optimization.
- **Right**: The optimized path of point `P`, following the desired 15 cm trajectory.

## Dependencies

This project uses the following Python libraries:

- `numpy` – For numerical operations
- `matplotlib` – For plotting and visualization
- [`pyswarm`](https://github.com/tisimst/pyswarm) – For PSO optimization

To install these dependencies, use:

```bash
pip install numpy matplotlib pyswarm
```

## Contributing

Contributions are welcome! Here’s how you can contribute:

1. Fork the repository.
2. Create your branch (`git checkout -b feature/new-feature`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature/new-feature`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

- **Taha Faghani** - taha.faghani@example.com
- GitHub: [tahafaghani](https://github.com/tahafaghani)

