# Practical workshop on Bayesian Hierarchical Models

## Agenda

1. Statistische Modellierung vs. Machine Learning
2. Unsicherheit beherrschen: Bayessche Modelle
    * Praxisteil I: Bayessche Lineare Modelle
3. Informationen Teilen: Bayessche Hierarchische Modelle
    * Praxisteil II: Bayessche Hierarchische Modelle

## Spin up the environment

```bash
docker build -t bhm_workshop .
```

```bash
docker run -p 8888:8888 \
           -v $(PWD)/data/:/home/jovyan/data/ \
           -v $(PWD)/praxisteil/:/home/jovyan/praxisteil/ \
           bhm_workshop
```

And then just copy paste the http://127.... (with token) into your browser.

If you want to add additional packages you can do so in two ways:
- Add them permanently by adding it to the requirements.txt.
- Install them in the jupyter notebook by executing `!pip install <YOUR PACKAGE>` in a cell.