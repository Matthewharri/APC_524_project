# APC_524_project

## Summary

Our project aims to provide an accessible and engaging way for people to quickly visualize animal tracking data from [MoveBank](https://www.movebank.org/cms/movebank-main), an open-source animal tracking database. It is Python-based and can be imported as a package for the user to run in a Jupyter notebook.

Tracks from the database are shown on top of an interactive world map, with the ability to view and toggle multiple tracks (if available), and additional information about the animal is sourced from Wikipedia and displayed.

## Usage

To create the conda environment, run
```
conda create --name geoVis environment.yml
```

To activate it,
```
conda activate geoVis
```

The interactive code example is located in a Jupyter notebook, which runs on data by [O'Mara, et. al](https://www.movebank.org/cms/webapp?gwt_fragment=page=studies,path=study312057662) from MoveBank. The notebook can be run with:
```
cd src/
jupyter notebook interactiveVisualizer.ipynb
```

## Notes for development
To run `nox` locally, install `nox` (if needed) with `conda install nox` and in the main directory, run
```
nox -s tests
```

To run the pre-commit hook (for syntax checks for example), in the main directory, run
```
pre-commit run -a
```
