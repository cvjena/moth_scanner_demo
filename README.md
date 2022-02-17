# Moth Scanner Demo
*This notebook visualizes the results of trained models (detector and classifier) for the moth scanner presented in the following [paper]*.

## Installation

We suggest using [miniconda]. All required libraries are listed in the `requirements.txt` and can be installed with `pip`:

```bash
conda create -n scanner_demo python~=3.8.0
conda activate scanner_demo
pip install -r requirements.txt
```

## Data and Model Weights

### Data
The [EU-Moths][1] dataset can be downloaded from the given URL. In this notebook, we assume that the uncropped version of it is located under `/home/korsch/Data/datasets/moths/eu_moths/uncropped/ORIGINAL`. Set the `root` attribute of the `Args` class accordingly when you create an instance of it to match the location of your dataset. Please consult this [GitHub repository][2] to get more information about the [MCC] dataset.

### Model Weights

Download the weights of the detector and the classifier and move them in the same directory as the jupyter notebook:
* [Classifier] (~ 84.7 MB)
* [Detector] (~ 78.8 MB)

*Password for both downloads: `Moth_Scanner`*

## Licence
This work is licensed under a [GNU Affero General Public License][agplv3].

[![AGPLv3][agplv3-image]][agplv3]

[agplv3]: https://www.gnu.org/licenses/agpl-3.0.html
[agplv3-image]: https://www.gnu.org/graphics/agplv3-88x31.png
[paper]: https://pub.inf-cv.uni-jena.de/search/Korsch21_DLP
[miniconda]: https://docs.conda.io/en/latest/miniconda.html
[1]: https://www.inf-cv.uni-jena.de/eu_moths_dataset
[2]: https://github.com/kimbjerge/MCC-trap/
[MCC]: https://github.com/kimbjerge/MCC-trap/tree/master/data
[Classifier]: http://ammod.inf-cv.uni-jena.de/sharing/U5wV185GT
[Detector]: http://ammod.inf-cv.uni-jena.de/sharing/gpqKZNVEp
