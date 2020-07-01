# Place cells

My project on place cells research.
I am studying how topological information about environment can be extracted from neurons alone.

The work heavily relies on [Cell Groups Reveal Structure of Stimulus Space](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1000205)
Curto C, Itskov V (2008) Cell Groups Reveal Structure of Stimulus Space.
PLOS Computational Biology 4(10): e1000205.

However, a better method for topological features extraction was applied;
I used [persistent homologies](https://en.wikipedia.org/wiki/Persistent_homology)
to calculate Betti numbers (i.e. number of holes). This yielded _good_ results
on the real (not synthetic/generated) dataset.

## Run

I recommend you to create a new virtual environment for the project

```bash
  python -m venv env
  source env/bin/activate
```

Then,

```bash
  pip install -r requirements.txt
```

```bash
  make run
```

This will run a jupyter notebook(lab) on localhost:8888
(warning: I disabled authentification for the jupyter notebook, so you may want
to avoid running it when connected to public networks, or you can just run
jupyter notebook normally by typing `jupyter lab` in terminal)

## Presentation (with images)

If you want a very short introduction to topology and this research, you can follow
[the link](https://docs.google.com/presentation/d/14w54qtytAnmYjUSET2NCNGnUpqrMwVsIfT9REbYE2Zc/edit?usp=sharing)
to see a presentation I have made to present the results of my work. The presentation
has all the information you need to get started.
