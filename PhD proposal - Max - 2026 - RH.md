# Background
---
Ultrasound-driven microbubbles are sensitive to the mechanical properties of their surrounding medium and can therefore act as local probes of high-frequency viscoelasticity. Previous work has demonstrated microbubble-based rheological characterisation using optical measurements of bubble dynamics, while acoustic and imaging studies have shown that bubble emissions and acoustic droplet vaporisation (ADV) dynamics can correlate with the properties of tissue-mimicking materials.

However, it remains to be established whether acoustic measurements alone can provide sufficiently independent information to estimate the viscoelastic properties of a surrounding medium, particularly when uncertainty in bubble size, shell mechanics and acoustic excitation is taken into account.

This project will investigate acoustic-only ADV-generated microbubble microrheology in homogeneous, isotropic, tissue-mimicking viscoelastic materials. It will determine which acoustic features provide useful information about the medium's elastic and dissipative properties, and whether these properties can be estimated reliably without optical measurements of bubble-radius dynamics.

# Research question
---
Can we estimate the effective shear modulus and viscosity of homogeneous, isotropic viscoelastic media from the acoustic emissions of a population of ultrasound-driven, ADV-generated bubbles?

# Hypothesis
---
The combination of a physically informed coated-nanodroplet model, appropriately selected ultrasound excitation and acoustic-emission features can enable the estimation of selected viscoelastic properties of a surrounding medium. Using complementary measurements across excitation frequencies or amplitudes may improve the separation of elastic and dissipative effects compared with single-condition, amplitude-based measurements.

The hypothesis will be tested by comparing recovered properties with independently characterised phantom values, quantifying uncertainty and evaluating whether increasingly complex bubble and tissue models improve estimation performance.

# Proposal
---
The **main objective** of the project is *to establish and experimentally validate a quantitative method for estimating selected high-frequency viscoelastic properties from ADV-generated microbubble acoustic emissions, and to determine its limits of identifiability and robustness.*

Nanodroplets will be embedded in gels with known properties and subjected to nonlinear ultrasound imaging. Their response and acoustic emissions will be modelled and various nonlinear imaging techniques will be assessed for their ability to produce measurable changes in the acoustic response of the microbubbles under a set of material parameters.

The acoustic emissions of the microbubbles will be measured using B-mode imaging and PCD and our segmented DWPT signal processing technique will be used to process the recordings and extract the desired signatures. We will develop and implement an inverse model to estimate the properties of the medium from these signatures. 

---
# Scope
---
1. Review current techniques used for microrheology at high strain rates.
2. Review current imaging and signal processing methods for microrheology using ultrasound contrast agents.
3. Model microbubble and ADV dynamics with a viscoelastic lipid coating in a viscoelastic medium using existing numerical models.
4. Identify how spectral features change as a function of material viscoelastic properties.
5. Model the acoustic emissions from ADV-generated microbubbles under various nonlinear imaging techniques while changing the material elasticity and viscosity.
6. Develop a signal processing strategy to extract features of interest.
7. Estimate medium properties based on acoustic emissions from microbubbles (inverse problem).
8. Implement nonlinear imaging techniques on Verasonics machine.
9. Measure acoustic emissions from nanodroplets experimentally.
    
# Workpackages and the timeline
**Start time - 1st of October 2026**

---

## WP1 [M1-M3]: Research gap and feasibility
---
[scope 1 & 2]

**Objective:** Establish the precise contribution and define the experimental operating range.

**Activities**
- Review high-strain-rate rheometry, acoustic microbubble rheology and acoustic feature-based tissue characterisation.
- Find limitations of these techniques (opacity, in vivo, high strain rates, spatial resolution).
- Show that coated microbubbles can be used to perform microrheology.
- Select the primary phantom, target parameters and candidate contrast agent.
- Define acoustic acquisition requirements, parameter ranges and reference rheometry.
- Confirm that no one has used spectral features to estimate material properties.

**Deliverables**
- A defensible research gap, a defined measurement problem and a feasibility specification.
- Identify material properties for numerical simulations.
- Identify the target medical application (prostate / liver fibrosis), find the materials and material properties to study.
  
## WP2 [M1-M6]: Forward model and identifiability
---
[scope 3 & 4]

Develop a model for coated nanodroplets in a viscoelastic medium. The model should capture the main physics of viscoelastic tissue and bubble shell dynamics. It is used as a forward model to identify spectral features of interest for estimating material properties.Finally, parameter identifiability will be investigated to establish which material parameters can be estimated from emissions (if the system is determined or under-determined).

**Objective:** Establish which material parameters can, in principle, be recovered.

**Activities**
- Research and develop a physically accurate and representative model for a coated nanodroplet in a viscoelastic medium.
- Compare simpler and more complex shell and tissue constitutive models.
- Perform a sensitivity analysis to determine how microbubble and tissue parameters ($G$, $\mu$, and fracttional order if a fractional model is taken, surrounding volume, heterogeneity) affect spectral features of acoustic emissions.
- Establish whether the measurements distinguish tissue elasticity from fractional-order dissipation?
- Identify spectral features that recover the desired tissue parameters with useful (calculated) undertainty and are feasibly measurable in vivo. These features should be unique: unique relationships between extracted features and each property.
- Investigate the effects of UCA size distribution; narrower vs larger distributions and how they affect the desired signatures.
- Test whether multi-frequency or multi-amplitude excitation adds independent information.

**Deliverables**
- A verified forward model for coated nanodroplets in a viscoelastic medium.
- Identified spectral features which are related to material properties $G$ and $\mu$, and possible $\alpha$ (fractional order).
- Article discussing the relationship between material properties and spectral features from a microbubble contrast agent in a viscoelastic medium.

## WP3 [M7-M10]: Nonlinear imaging sequence
---
[scope 5]

Assess nonlinear imaging techniques to improve sensitivity and specificity of selected spectral features. Develop a signal processing strategy to extract these features.

**Activities**
- Simulate nonlinear imaging strategies and resulting microbubble acoustic emissions in viscoelastic medium (use the physical and numerical models developed in WP2).
- Identify nonlinear technique that has the greatest improvement on the sensitivity and specificity of the measured features.

**Deliverables**
- Numerical simulations of nonlinear imaging methods and microbubble acoustic emissions.
- Nonlinear imaging sequence that uniquely connects features from acoustic emissions from cavitation to properties of the surrounding medium.
- Article presenting discovered connection between features from acoustic emissions and medium properties and optimal nonlinear protocol.


## WP 4 [M10-M16]: Inverse problem
---
[scope 6 & 7]

**Objectives:** Estimate material parameters using extracted features from acoustic emissions of microbubbles in a viscoelastic medium.

**Activities**
- Identify and implement anti-aliasing algorithm, and more robust clustering technique for the published discrete wavelet packet transform (DWPT) algorithm to decompose acoustic emissions into their components in time domain based on their temporal-spectral features.
- Apply the improved DWPT algorithm to extract desired features from simulated UCAs in different tissues (UCAs are excited by the nonlinear sequence developed in WP3, using physical model in WP2).
- develop an inverse method to estimate the material properties from extracted feastures (decomposed time-series or extracted spectral features or both). The inverse methos can be classical statistical approaches or ML-based (TBD)
- characterise the spatial resolution of this approach.
- if and how this approach can be extended for spatial mapping of tissue properties 

**Deliverables**
- Signal processing pipeline for extracting features identified in WP2.
- Micro-rheology data validating the proposed solution (nonlinear imaging + UCA for localised rheology)
- Article presenting a novel method for acoustic cavitation rheometry using acoustic emissions from single bubble dynamics.

## WP 5 [M16-M24]: Phantom validation and thesis 
---
[scope 8 & 9]

Experimental validation and writeup.

**Activities**
- Produce homogeneous hydrogels with consistent viscoelastic properties, potentially replicating the properties of the desired tissue specified in WP1.
- Estimate rheological properties of the hydrogels.
- Embed microbubble contrast agents into gels. Apply nonlinear imaging sequence to samples with an imaging ultrasound probe and collect acoustic emissions using PCD.
- Characterise the properties of the hydrogels using algorithm developed in WP4.
- Write up thesis.

**Deliverables**
- Article presenting a novel acoustic cavitation rheometry technique on hydrogels / [liver/prostate] tissue.
- PhD thesis.

### Additional papers
- Review article on acoustic cavitation microrheology.

---
## Novelty and expected contribution
---
The expected contributions are:

1. Establish which measurable acoustic features are sensitive to the viscoelastic properties of the surrounding medium and which provide independent information about elasticity and dissipation.
2. Quantify parameter identifiability and estimation uncertainty in the presence of uncertainty in bubble size, shell mechanics and acoustic excitation.
3. Determine whether nonlinear excitation and complementary acoustic measurements improve the accuracy and robustness of material-property estimation compared with simpler measurement protocols.
4. Validate the approach in independently characterised tissue-mimicking phantoms and evaluate its potential for spatially resolved measurements.

The principal novelty is the development and validation of a **quantitative acoustic-only inference framework**, rather than the use of microbubbles, nonlinear emissions or cavitation rheology in isolation.