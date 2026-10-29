# BayesCrash

![The reverend Thomas Bayes](https://upload.wikimedia.org/wikipedia/commons/d/d4/Thomas_Bayes.gif)

This Jupyter notebook is essentially a crash course in Bayesian inference with applications to geophysical data assimilation, machine learning, geostatistics, and inverse modeling, where I try to cover the most important probabilistic ideas and numerical methods based on lectures we have given for the Master/PhD course Geophysical Data Science GEO4300/GEO9300 led by Norbert Pirk [@norberp](https://www.github.com/norberp) at the University of Oslo. It corresponds roughly to a 2-hour guest lecture that I give in this course, but the notebook should be completely self-contained and is thus arguably well suited for self-study. The geophysical data science course we offer [uio.no/studier/emner/matnat/geofag/GEO4300/](https://www.uio.no/studier/emner/matnat/geofag/GEO4300/) covers a wide range of data science topics with relevance to research in geophysics of the entire Earth system (not just fossils) and beyond, while being almost entirely based on modern and open programming tools in the form of Jupyter notebooks and the Python programming language.

Please reach out to me, Kristoffer Aalstad (kristoffer.aalstad@geo.uio.no), if you spot any typos, errors, or have any feedback.

# Running the notebook

## In the browser (no installation)

Open the notebook directly in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/krisaalstad/BayesCrash/blob/main/BayesCrash.ipynb)

## Locally with uv (recommended)

The environment is managed with [uv](https://docs.astral.sh/uv/), which also installs the right Python version for you. With uv installed, run:

```bash
git clone https://github.com/krisaalstad/BayesCrash.git
cd BayesCrash
uv sync
```

Then open the `BayesCrash` folder in [Positron](https://positron.posit.co/) or VS Code, select the project's `.venv` interpreter, and open `BayesCrash.ipynb`. If you prefer JupyterLab, run `uv run --with jupyterlab jupyter lab` instead.

The notebook is tested with Python 3.14, and any Python version from 3.11 upwards should work.

# References

Freely available as PDFs online:

Evensen et al. (2022): Data Assimilation Fundamentals, [doi:10.1007/978-3-030-96709-3](https://doi.org/10.1007/978-3-030-96709-3)

Gelman et al. (2013): Bayesian Data Analysis (3rd ed.), [doi:10.1201/b16018](https://doi.org/10.1201/b16018)

Murphy (2023): Probabilistic Machine Learning: Advanced Topics, [probml.github.io/pml-book/book2.html](https://probml.github.io/pml-book/book2.html)

S&auml;rkk&auml; and Svensson (2023): Bayesian Filtering and Smoothing (2nd ed.), [doi:10.1017/9781108917407](https://doi.org/10.1017/9781108917407)

As far as I know not free, but also great resources:

Otsuka (2023): Thinking about Statistics, [doi:10.4324/9781003319061](https://doi.org/10.4324/9781003319061)

McElreath (2020): Statistical Rethinking (2nd ed.), [doi:10.1201/9780429029608](https://doi.org/10.1201/9780429029608)

I would also warmly recommend checking out Richard McElreath's fantastic [lectures](https://youtube.com/playlist?list=PLDcUM9US4XdPz-KxHM4XHt7uUVGWWVSus) on YouTube.

# Acknowledgements

We kindly thank all open data providers. Data from the Blindern meteorological station (SN18700) on the University of Oslo campus was obtained from the Norwegian Meteorological Institute through [https://seklima.met.no/](https://seklima.met.no/). GISS Surface Temperature Analysis (GISTEMP) data was obtained from the NASA Goddard Institute for Space Studies via [https://data.giss.nasa.gov/gistemp/](https://data.giss.nasa.gov/gistemp/).
