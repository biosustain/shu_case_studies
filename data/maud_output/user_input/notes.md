# Model of E. coli glycolysis

## Notes about specific enzymes 
### PGI
https://www.biocyc.org/gene?orgid=ECOLI&id=PGLUCISOM#tab=RXNS 

Biocycpoints to this paper https://pubmed.ncbi.nlm.nih.gov/7004378/ which says
that G6P inhibits the enzyme PGI but doesn't say the mechanism. Should this be
included in the model, and with what mechanism?

### PFKA
https://biocyc.org/gene?orgid=ECOLI&id=EG10699#tab=RXNS 

Biocycpoints to this paper https://pubmed.ncbi.nlm.nih.gov/4268865/ which says
that F6P inhibits the enzyme PFKA but doesn't say the mechanism. Should this be
included in the model, and with what mechanism?

GDP is an allosteric activator but is not currently included in this model.

Modelled modifiers:

- Activators (Allosteric)	ADP
- Inhibitors (Allosteric)	phosphoenolpyruvate

Not modelled:

- Activators (Allosteric) GDP
- Activators (Non-Allosteric) β-D-fructofuranose 6-phosphate

### PFKB
https://biocyc.org/gene?orgid=ECOLI&id=EG10700#tab=RXNS

Modelled modifiers:

- Inhibitors (Allosteric) ATP
- Inhibitors (Competitive) β-D-fructofuranose 1,6-bisphosphate

Not modelled:

- Activators (Allosteric) phosphocarrier protein HPr
- Inhibitors (Unknown Mechanism) citrate, GTP, K+, phosphate, phosphoenolpyruvate

### FBAA
https://biocyc.org/gene?orgid=ECOLI&id=EG10282#tab=RXNS

Not modelled:

- Activators (Unknown Mechanism) ammonium, K+
- Inhibitors (Unknown Mechanism) EDTA, Ni2+

### FBAB
https://biocyc.org/gene?orgid=ECOLI&id=G7129#tab=RXNS

Not modelled:

- Activators (Unknown Mechanism) citrate
- Inhibitors (Irreversible) borohydride

### TPI
https://biocyc.org/gene?orgid=ECOLI&id=EG11015#tab=RXNS

Did not include competitive inhibition by 2-phosphoglycolate as that metabolite
is not in the model.

### GAPD
https://biocyc.org/gene?orgid=ECOLI&id=EG10367#tab=RXNS

Not modelled:

- Activators (Unknown Mechanism) arsenate
- Inhibitors (Unknown Mechanism) iodoacetate

### PGK
https://biocyc.org/gene?orgid=ECOLI&id=EG10703#tab=RXNS

### PGM
https://biocyc.org/gene?orgid=ECOLI&id=EG11699#tab=RXNS

Not modelled:

- Inhibitors (Unknown Mechanism) K+, phosphate, vanadate

### ENO
https://biocyc.org/gene?orgid=ECOLI&id=EG10258#tab=RXNS

Not modelled:

- Inhibitors (Unknown Mechanism) fluoride
