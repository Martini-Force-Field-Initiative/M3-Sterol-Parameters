# Supporting Information for: Parameterization of cholesterol for the Martini 3 coarse grained force field

by Luís Borges-Araújo [^1][^2]; Ana C. Borges-Araújo [^1]; Tugba Nur Ozturk[^3]; Daniel P. Ramirez-Echemendia[^4]; Balázs Fábián [^5]; Timothy S. Carpenter[^3]; Sebastian Thallmair [^6]; Jonathan Barnoud [^7][^8]; Helgi I. Ingólfsson[^3]; Gerard Hummer [^5]; D. Peter Tieleman[^4]; Siewert J. Marrink [^9]; Paulo C. T. Souza [^2]; Manuel N. Melo [^1]

[^1]: Instituto de Tecnologia Química e Biológica António Xavier, Universidade Nova de Lisboa, Av. da República, 2780-157, Oeiras, Portugal;
[^2]: Molecular Microbiology and Structural Biochemistry, UMR 5086 CNRS & University of Lyon, 7 Passage du Vercors, Lyon F-69367, France;
[^3]: Physical and Life Sciences (PLS) Directorate, Lawrence Livermore National Laboratory, Livermore, CA, 94550, USA;
[^4]: Centre for Molecular Simulation and Department of Biological Sciences, University of Calgary, Alberta, Canada;
[^5]: Department of Theoretical Biophysics, Max Planck Institute of Biophysics, Max-von-Laue Straße 3, 60438 Frankfurt am Main, Germany;
[^6]: Frankfurt Institute for Advanced Studies, Ruth-Moufang-Straße 1, 60438 Frankfurt am Main, Germany:
[^7]: Centre for Computational Chemistry, School of Chemistry, University of Bristol, Bristol, UK;
[^8]: CiTIUS Intelligent Technologies Research Centre, University of Santiago de Compostela, Santiago de Compostela, Spain.
[^9]: Groningen Biomolecular Sciences and Biotechnology Institute, University of Groningen, Nijenborgh 7, 9747 AG Groningen, The Netherlands

* Corresponding authors:   Manuel N. Melo - m.n.melo@itqb.unl.pt; Paulo C.T.Souza - paulo.telles-de-souza@ibcp.fr

# Cite us!
If you use these parameters please cite the following article:
   Borges-Araújo, L. et al. Martini 3 Coarse-Grained Force Field for cholesterol. (2023) doi: https://doi.org/10.1021/acs.jctc.3c00547


# Contents
This github repository contains supporting information for the parameterization of cholesterol for the Martini 3 coarse grained force field. You can find here intermediary development cholesterol parameters, as well as the final Martini 3 cholesterol model. An `insane.py` script containing the new Martini 3 cholesterol model is also supplied. Alternatively, you can add the following entry to your own `insane.py`:
```
# Sterols
moltype = "sterol"
lipidsx[moltype] = (      0,   1,   0,   0,  1,   0, 0.5, 0.5,   0,  0)
lipidsy[moltype] = (      0,   0,   0,   0,  0,   0,   0,   0,   0,  0)
lipidsz[moltype] = (    5.3, 4.5, 3.9, 3.3,  3, 2.6, 4.5, 2.6, 1.4,  0)
lipidsa.update({
    "CHOL": (moltype, " ROH  R1  R2  R3  R4   -  R5  R6  C1  C2 "),
})
```

