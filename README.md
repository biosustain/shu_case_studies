# Shu cases studies

This repository contains notebooks for reproducing the two figures in the manuscript _Shu: Visualization of high dimensional Biological Pathways_.

## Figure 1: maud case study

The kinetic model can be found at [`models/maud_ecoli_glycolysis_and_ppp`](./models/maud_ecoli_glycolysis_and_ppp). The output of [Maud](https://github.com/biosustain/Maud)
is provided at [`data/maud_output`](./data/maud_output).

To reproduce the output generation (might take a day):

```bash
# install the bayesian kinetic modeling software
pip install maud-metabolic-models==0.4.0.2
install_cmdstan
# sample a posteriori distribution
maud sample models/maud_ecoli_glycolysis_and_ppp
```

The notebook [`notebooks/1_shu_maud.ipynb`](./notebooks/1_shu_maud.ipynb)
performs the required data wrangling using `pandas` (without [`ggshu`](https://pypi.org/project/ggshu)) to produce the
input for [`shu`](https://github.com/biosustain/shu) (click on "Data" at https://biosustain.github.com/shu)
at [`data/maud_output.metabolism.json`](./data/maud_output.metabolism.json). The network map is at [`maps/ecoli_map.json`](./maps/ecoli_map.json).

## Figure 2: omics case study

The notebook [`notebooks/2_shu_omics.ipynb`](./notebooks/2_shu_omics.ipynb)
arranges the omics data, computes the flux sampling (using `models/iCLAU786.xml` and `models/eciICLAU786.xml`)
and uses [`ggshu`](https://pypi.org/project/ggshu) to produce the input for [`shu`](https://github.com/biosustain/shu)
at [`data/omics.metabolism.json`](./data/omics.metabolism.json).

The map is a custom one for Clostridium autoethanogenum and is available at [`data/case_study_map.json`
](./maps/cauto_map.json).