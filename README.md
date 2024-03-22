D2IM_Prototype
==============================

A proof of concept Deep Learning model to predict displacements from greyscale XCT scans of mechanical experiments.

More information about the project can be found at the following preprint - please cite this paper if using and of the code or data in your own projects: 
Soar, P. and Tozzi, G., 2023. Data-driven image mechanics (D2IM): a deep learning approach to predict displacement and strain fields from undeformed X-ray tomography images-Evaluation of bone mechanics. bioRxiv, pp.2023-09. https://doi.org/10.1101/2023.09.21.558878

The dataset used comprises slices of porcine vertebra. The original 3D scans of the images can be found at:
Dall'Ara, Enrico; Palanca, Marco (2021). Data for paper "MicroFE models of porcine vertebrae with induced bone focal lesions: validation of predicted displacements with Digital Volume Correlation". The University of Sheffield. Dataset. https://doi.org/10.15131/shef.data.16732441
Mask input was generated from these scan slices. Target displacements (u,v,w) were obtained using the DIC/DVC software SPAM (https://www.spam-project.dev/).
'Clinical' folder contains a few examples used for testing the sensitivity of the D2IM model to lower resolution input. The clinical scans these slices were extracted from were collected at the CT Scan Department, Northern General Hospital, Sheffield.


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
