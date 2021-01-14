# Practical workshop on Bayesian Hierarchical Models (BHMs)

## Agenda

Theory 

Practicing

## Spin up the environment

```bash
docker build -t bhm_workshop .
```

```bash
docker run -p 8888:8888 \
           -v $(PWD)/data/:/home/jovyan/data/ \
           -v $(PWD)/notebooks/:/home/jovyan/notebooks/ \
           pymc3
```

And then just copy paste the http://127.... into your browser.

If you want to add additional packages you can do so in two ways:
- Add them permanently by adding it to the requirements.txt.
- Install them in the jupyter notebook by executing `!pip install <YOUR PACKAGE>` in a cell.