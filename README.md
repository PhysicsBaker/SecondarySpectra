# SecondarySpectra
Secondary spectra from evaporating black holes for SM and BSM benchmarks

These secondary spectra are used in [2210.02805](https://arxiv.org/abs/2210.02805), which you should read for further details

All spectra were generated using [Pythia8](https://pythia.org/)

If these spectra are used in a published work, please cite [2210.02805](https://arxiv.org/abs/2210.02805)

---

**sp-sm** contains the secondary spectra for the standard model particles using the format sp-sm-pid, where pid is the Monte Carlo Particle Numbering Scheme used by the PDG, see [here](https://pdg.lbl.gov/2022/reviews/rpp2022-rev-monte-carlo-numbering.pdf)

The columns give the:

(1) primary particle energy\
(2) secondary particle energy\
(3) # photons\
(4) # electrons\
(5) # electron neutrinos\
(6) # muon neutrinos\
(7) # tau neutrinos\
(8) # protons

per parent particle per energy bin, with energies in GeV

The bins are evenly spaced in log space, with the secondary particle energy values giving the centre of the bin 

---

**sp-mssm** gives the same information for the MSSM benchmark defined in [2210.02805](https://arxiv.org/abs/2210.02805)

It also contains the secondary spectra for the 125 GeV Higgs boson (pid 25), since its properties are slightly different to the SM Higgs boson

These files have an extra column:

(9) # lightest supersymmetric particles, in this case ~chi_1^0 (pid 1000022)

---

**Spheno.spc.mssm** is the spectrum file used to generate the files in sp-mssm, which was generated using [SPheno](https://spheno.hepforge.org/)

---

**d2NdEfdtDataSM.m** is a Mathematica file containing the total secondary photon spectra following equation (5) in [2210.02805](https://arxiv.org/abs/2210.02805)

Each triplet of values gives {Log10(MBH [g]), Log10(Ef [GeV]), Log10(d2NdEfdt [GeV^-1 s^-1])), where Ef is the energy of the secondary photon

---

**d2NdEfdtDataMSSM.m** is the same for the MSSM benchmark
