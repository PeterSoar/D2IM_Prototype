D2IM Prototype
==============================

A proof of concept Deep Learning model to predict displacements from greyscale XCT scans of mechanical experiments.

More details can be found in the following paper - please cite this paper if using the code or data in your own projects:

"Data-driven image mechanics (D2IM): a deep learning approach to predict displacement and strain fields from undeformed X-ray tomography images - Evaluation of bone mechanics"

by Peter Soar, Marco Palanca, Enrico Dall'Ara and Gianluca Tozzi submitted to publication in Extreme Mechanical Letters, 2024. Currently available as a preprint at: https://www.biorxiv.org/content/10.1101/2023.09.21.558878v1.abstract

Mask input was generated from these scan slices. Target displacements (u,v,w) were obtained using the DIC/DVC software SPAM (https://www.spam-project.dev/).
'Clinical' folder contains a few examples used for testing the sensitivity of the D2IM model to lower resolution input. The clinical scans these slices were extracted from were collected at the CT Scan Department, Northern General Hospital, Sheffield.

An interactive version of D2IM can be found hosted on Kaggle at: https://www.kaggle.com/code/petersoar/d2im-prototype
The data is also hosted on Figshare at: https://doi.org/10.6084/m9.figshare.25404220.v1

Project Organization
------------

    ├── LICENSE
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── Clinical       <- Resized and clinical test images.
    │   ├── Input          <- Derived input Images.
    │   └── Target         <- GRound Truth Images.
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── reports            <- Generated analysis and predictions.
    │   ├── figures        <- Generated graphics and figures used in the paper.
    │   └── predictions    <- Supplemental images showing the predictions and error of all three displacement components on the test data.
    │   
	└──  requirements.txt  <- The requirements file for reproducing the analysis environment, e.g.


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
