
# Pokemon Team Optimizer for Pokemon Black & White: A Data Science Approach

## Overview

This project utilizes data science and optimization algorithms to identify the best possible team of Pokemon you can have in Pokemon Black & White. The criteria for "best" can be tailored to your specific needs, be it a well-rounded team, a team focusing on a specific type, or any other conditions you'd like to impose.

## Table of Contents

- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Data](#data)
- [Contributing](#contributing)
- [Credits](#credits)
- [License](#license)

## Requirements

- Python 3.x
- numpy
- pandas
- PuLP 1.6.8

## Installation

1. Clone this repository.

    ```bash
    git clone https://github.com/yourusername/pokemon-team-optimizer.git
    ```

2. Navigate to the project directory.

    ```bash
    cd pokemon-team-optimizer
    ```

3. Install the required packages.

    ```bash
    pip install numpy pandas pulp==1.6.8
    ```

## Usage

Run the script to get the optimized Pokemon team:

```bash
python optimizer.py
```

## Data

The data used in this project is a combination of several CSV files that include Pokemon stats, types, and other metrics:

- `Pokemon.csv`: General Pokemon data including stats.
- `Pokemon Type Chart.csv`: Data that defines the type advantages and disadvantages.

Data is loaded from these files and processed in the main Python script to produce an optimized Pokemon team.

```python
poke_df = pd.read_csv("../input/pokemon/Pokemon.csv")
typeChart = pd.read_csv("../input/pokemon-types/Pokemon Type Chart.csv", index_col = [0])
```

## Contributing

We welcome contributions! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to contribute.

For any questions or suggestions, please open an issue or submit a pull request. Enjoy optimizing your Pokemon team!
