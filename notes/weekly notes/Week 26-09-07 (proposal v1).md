# Background

### Applications [find more literature for high frequency applications]
>[!NOTE] Characterising fibrin density
>- correlated with several pathological processes e.g. fibrosis (scarring of the liver)
>- thrombus stiffness can be estimated by fibrin density
>- characterising fibrin density can therefore be used to understand tissue health and monitor disease progression.

> [!PDF|yellow] [[kaushik_adv_tissue_characterisration_transfer_learning.pdf#page=1&selection=176,0,179,38&color=yellow|kaushik_adv_tissue_characterisration_transfer_learning, p.1]]
> > PATHOLOGICAL processes frequently alter the structural and mechanical properties of soft tissues, serving as key biomarkers for early disease detection

>[!NOTE] Characterising physical properties
>- Physical properties of soft tissues are not known for strain rates in the MHz range at which microbubbles are driven.
>- The elasticity, shear modulus, and viscosity can be measured using rheology which has a wide range of industrial and biomedical applications.
>- Detecting changes in In vivo properties (characterise resolution and sensitivity). 

> [!PDF|yellow] [[rezaei_microbubble_acoustic_cavitation_soft_matter.pdf#page=21&selection=18,44,30,47&color=yellow|rezaei_microbubble_acoustic_cavitation_soft_matter, p.21]]
> > While the physical properties of soft tissues are widely available for strain rates in the range of 1 to 10 s−1, they are largely unknown for strain rates of 106 s−1 at which the microbubbles are typically driven.

- [find more applications for high frequency and microrheology]
# Research question

How can microbubbles and nonlinear imaging be used for microrheology for characterising viscoelastic properties of [collagen/fibrin/hydrogels/tissues].

- which soft tissues?
# Proposal

Microbubbles will be embedded in gels with known properties and subjected to nonlinear ultrasound imaging. Their response and acoustic emissions will be modelled [which models?] and various nonlinear imaging techniques [which ones?] will be assessed for their ability to produce measurable changes in the acoustic response of the microbubbles under a set of material parameters [under which material parameters?].

The acoustic emissions of the microbubbles will be measured using B-mode imaging and PCD and signal processing techniques [which ones?] will be used to estimate the properties of the medium. The B-mode data can be reconstructed after signal processing to obtain spatial information on the material properties. 
# Scope

- Review current techniques used for microrheology at high strain rates. [distinguish between these and bulk rheology and low strain rates (make block diagram for proposal.)] 
- Review current imaging and signal processing methods for microrheology using ultrasound contrast agents.
- Model microbubbles dynamics with a viscoelastic lipid coating in a viscoelastic medium using existing numerical models.
- Model the acoustic emissions from microbubbles under various nonlinear imaging techniques while changing the material elasticity and viscosity [which one? (definity or sonovue?)].
- Identify how spectral features change as a function of material viscoelastic properties.
- Develop a signal processing strategy to extract features of interest.
- Estimate medium properties based on acoustic emissions from microbubbles (inverse problem).
- Implement nonlinear imaging techniques on Verasonics machine.
- Measure acoustic emissions from commercially available [which one?] microbubbles experimentally.
- Implement custom beamforming algorithm to perform microrheology on a live sample?
# Timeline [add months to each deliverable]

- Add low-level detail to each item.
- Which models? Which algorithms?
### Establish a model for micobubbles in viscoelastic media

- Model bubble dynamics.
- Model scattered pressure from microbubbles.
- Perform parametric studies.
- Establish a relationship between US scattering, ultrasound parameters, microbubble parameters, and viscoelastic parameters of the medium.

### Extract spectral features from microbubble emissions

- Identify how spectral features change depending on medium properties.
- Assess nonlinear imaging strategies on extracting spectral features.

### Estimate microrheology parameters from microbubble emissions

- Review approaches for solving the inverse problem

### Experimental work

- Embed microbubbles in gels. 

---
# Novelty

- Highlight novelty of the work.
- First work package is not completely new. Find exact differences between planned work and existing work [complete lit review].