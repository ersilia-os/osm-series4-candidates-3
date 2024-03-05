# osm-series4-synthesis-round2
New round of generative synthesis for new Series 4 compounds based on experimental validations from previous work

## Tasks
1. We have curated all the availabe information on OSM compounds, including the experimental validations from Evariste and ersilia (2022)
2. We have built new AI/ML predictive models using ZairaChem (Turon, Hlozek et al, 2023) and [ChemPFN](https://github.com/ersilia-os/ensemble-tabpfn) with excellent accuracies (AUROC > 0.8)
3. We have used ChemSampler v0.1 (now [archived](https://github.com/ersilia-os/chem-sampler-legacy)) to search the chemical space for new molecular candidates
4. We have filtered the candidates with a list of constraints according to the requeriments of OSM (see below)

### Constraints for molecule selection

- Keep the triazolopirazine core + right hand substituent (as we agreed we only wanted small modifications on the left one)
- High predicted activity (at least, < 2.5 uM)
- Molecules with a predicted half-life (T1/2) < 0.5. According to their definition (Excretion tab) of halflife, the closer to 1, the shorter halflife, so in this case we go for a longer half-life (results from ADMETLab2)

## Results
We have identified a set of 19 candidates for experimental testing.

## License
All the code developed is licensed under a GPLv3 License. Content is released under a CC-BY 4.0.
