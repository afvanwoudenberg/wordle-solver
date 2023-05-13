# Wordle Solver

This repository contains a Jupyter notebook called `wordle.ipynb` that builds a decision tree that can be used to solve [Wordle](https://www.nytimes.com/games/wordle/index.html) games. It also shows how to traverse this decision tree using a simple user interface. A second notebook called `wordle_app.ipynb` only contains this user interface and loads the decision tree from file. You can run `wordle_app.ipynb` using Voila to turn this solver into a standalone web app.

## Getting Started

### Prerequisites

* [Anaconda](https://www.anaconda.com/distribution/) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html) must be installed on your machine.
* You should have basic knowledge of using Anaconda or Miniconda.

### Installing

1. Clone the repository:
```bash
git clone https://github.com/afvanwoudenberg/wordle-solver.git
```

2. Navigate into the project folder:
```bash
cd wordle-solver
```

3. Create the conda environment from the environment.yml file:
```bash
conda env create -f environment.yml
```

4. Activate the conda environment:
```bash
conda activate wordle-solver
```

5. Start Jupyter Notebook:
```bash
jupyter notebook
```

6. Open `wordle.ipynb` in the browser and run the notebook. Running all cells will (re)create a `wordle.json` file that represents the decision tree. Open `wordle_app.ipynb`to use this decision tree to solve Wordle puzzles.

### Using Voila

To use the `wordle_app.ipynb` notebook as a standalone Wordle solver web app using Voila:

1. Install Voila using conda: <br> 
(You can skip this step if you've created an environment from the [environment.yml](environment.yml) file)

```bash
conda install -c conda-forge voila
```

2. Launch Voila with the notebook:

```bash
voila wordle_app.ipynb
```

3. Your wordle solver app should now be running at http://localhost:8866/

### Links

Binder file: <a href="https://mybinder.org/v2/gh/afvanwoudenberg/wordle-solver/main?urlpath=%2Fvoila%2Frender%2Fwordle_app.ipynb">![Binder](https://mybinder.org/badge_logo.svg)</a>

Blog post: https://aswinvanwoudenberg.com/posts/draining-the-fun-out-of-wordle/

## Author

Aswin van Woudenberg ([afvanwoudenberg](https://github.com/afvanwoudenberg))

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
