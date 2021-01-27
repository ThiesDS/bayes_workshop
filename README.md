# Practical workshop on Bayesian Hierarchical Models

## Agenda

1. Theorie
    1. Machine Learning vs. Statistische Modellierung
    2. Grundlagen der Bayesschen Modellierung
    3. Pymc3 – Ein probabilistisches Programmierframework

2. Praxis
    1. Unsicherheit beherrschen: Bayessche Lineare Modelle
    2. Informationen teilen: Bayessche Hierarchische Modelle

## Spin up the environment

Install docker on your environment following [these](https://docs.docker.com/get-docker/) instructions.

After having installed docker, build the image as follows (this needs to be done only once):

```bash
docker build -t bhm_workshop .
```

Run the container with the following command:

```bash
docker run -p 8888:8888 \
           -v $(PWD)/data/:/home/jovyan/data/ \
           -v $(PWD)/2_praxis/:/home/jovyan/praxis/ \
           bhm_workshop
```

And then just copy paste the http://127.... (with token) into your browser.

If you want to add additional packages you can do so in two ways:
- Add them permanently by adding it to the requirements.txt.
- Install them in the jupyter notebook by executing `!pip install <YOUR PACKAGE>` in a cell.