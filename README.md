# Practical workshop on Bayesian Hierarchical Models

## Agenda

1. Theorie
    1. Machine Learning vs. Statistische Modellierung
    2. Bayessche Grundlagen
    3. Coin Flip Beispiel
    4. Pymc3

2. Praxis
    1. Teil I: Unsicherheit beherrschen: Bayessche Lineare Modelle
    2. Teil II: Informationen teilen: Bayessche Hierarchische Modelle

## Spin up the environment

Install docker on your environment following [these](https://docs.docker.com/get-docker/) instructions.

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