# Day 4 – Avatar Day - the Strengths and Limitations of 3D

Thursday, Aug 27, 2026

* 09:00 AM – 10:30 AM o Lecture X: 3D and Web-Based Visualization; A Geller
* 10:30 AM – 11:00 AM o BREAK
* 11:00 AM – 12:00 PM o Problem V: Firefly; A Geller
* 12:00 PM – ??:?? PM o BREAK

## Workshop on Firefly

In this workshop, we will explore the [Firefly](https://firefly.rcs.northwestern.edu/) visualization tool and learn how to use Firefly to visualize, explore and make selections on your data.  This workshop assumes a familiarity with Python.

### Installation

I recommend that you create a new environment for installing Firefly.  I provide commands below to do this with conda.  In the commmands below, replace `<envname>` below with a name for your environment.

(I included a few extra packages here that I used for the exercise to download and analyze the Gaia data.  If you just want to work with firefly in a notebook, you can simply install `python`, `jupyter` and `firefly`.)

```
conda create -n <envname> python=3.14 numpy hdbscan astroquery astropy matplotlib jupyter
conda activate <envname>
pip install firefly
```

If you need to register your Jupyter kernel (e.g., for use in VS Code):

```
python -m ipykernel install --user --name <envname> --display-name "<envname>"
```
### Exercise

1. Download/generate/use your own data that has x,y,z and other attributes.
    - *Suggestion:* Gaia data (e.g., for a galactic open cluster)
2. Ingest this into Firefly and explore it in a Jupyter notebook.
    - Make sure to include attributes to color/filter by.
4. Use the data selection tool to select a portion of your data using Firefly.
5. Create a plot of these selected data using Python.
6. Share the result with us!


### Notes

- When selecting data in Firefly, you may need to adjust the size (and distance) of the selection sphere so that it matches the size of the data region you plan to select.  You may need to explore your data outside of Firefly to understand the size of the region.  In Firefly, selected points change color to indicate that they are within the selection sphere.
- Firefly is still in active development.  If you like using it, consider checking back on our [GitHub repo](https://github.com/ageller/Firefly) or [PyPI page](https://pypi.org/project/firefly/) for new releases.


*The contents of this directory were copied here from [Aaron's CIERA_DSFP_2026 GitHub repo](https://github.com/ageller/CIERA_DSFP_2026) on Aug. 28, 2026.*