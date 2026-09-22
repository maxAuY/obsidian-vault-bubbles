# Background

### Applications

>[!NOTE] Multidisciplinary applications
>- Cavitation rheology has applications across several fields such as biology, chemistry, materials, and mechanics.
>- It can be used to characterise both fluids and solids.
>- In medicine, it is often used to quantitatively characterise disease progression by monitoring tissue damage and tissue properties.

> [!PDF|yellow] [[barney_2020_cavitation_in_soft_matter.pdf#page=7&selection=4,0,4,22&color=yellow|barney_2020_cavitation_in_soft_matter, p.7]]
> > Emerging Opportunities [Section highlighting applications in physics, biology, and chemistry.]

> [!PDF|yellow] [[barney_2020_cavitation_in_soft_matter.pdf#page=1&selection=112,0,114,27&color=yellow|barney_2020_cavitation_in_soft_matter, p.1]]
> > In solids, cavitation can occur in the solid itself or in liquid phases within a solid, such as water within a swollen hydrogel or tissue.

>[!NOTE] Characterising fibrin density
>- Fibrin density is correlated with several pathological processes e.g. fibrosis (scarring of the liver)
>- Thrombus stiffness can be estimated by fibrin density
>- Characterising fibrin density can therefore be used to understand tissue health and monitor disease progression.

> [!PDF|yellow] [[kaushik_adv_tissue_characterisration_transfer_learning.pdf#page=1&selection=176,0,179,38&color=yellow|kaushik_adv_tissue_characterisration_transfer_learning, p.1]]
> > PATHOLOGICAL processes frequently alter the structural and mechanical properties of soft tissues, serving as key biomarkers for early disease detection

>[!NOTE] Characterising physical properties
>- Physical properties of soft tissues are not known for strain rates in the MHz range at which microbubbles are driven.
>- The elasticity, shear modulus, and viscosity can be measured using rheology which has a wide range of industrial and biomedical applications.
>- Detecting changes in In Vivo properties (characterise resolution and sensitivity). 
>- Measuring rheology of soft tissues at high strain rates for modelling microbubbles for imaging and therapy.

> [!PDF|yellow] [[rezaei_microbubble_acoustic_cavitation_soft_matter.pdf#page=23&selection=9,0,16,71&color=yellow|rezaei_microbubble_acoustic_cavitation_soft_matter, p.23]]
> > Ultrasound contrast agents (UCAs) are widely used in medical imaging to enhance contrast and improve medical diagnosis, e.g. for organ perfusion imaging or to monitor hypervascularization in and around tumors [26], [27]. Additionally, UCAs are intensively investigated for their ultrasound-mediated therapeutic potential. Microbubbles can indeed increase the permeation of endothelial layers, resulting in the local delivery of drugs or genes through pore formation [28], [29].

> [!PDF|yellow] [[rezaei_microbubble_acoustic_cavitation_soft_matter.pdf#page=21&selection=18,44,30,47&color=yellow|rezaei_microbubble_acoustic_cavitation_soft_matter, p.21]]
> > While the physical properties of soft tissues are widely available for strain rates in the range of 1 to 10 s−1, they are largely unknown for strain rates of 106 s−1 at which the microbubbles are typically driven.

> [!PDF|yellow] [[rezaei_microbubble_acoustic_cavitation_soft_matter.pdf#page=24&selection=13,75,15,75&color=yellow|rezaei_microbubble_acoustic_cavitation_soft_matter, p.24]]
> > One major issue that remains is that the use of any of these models requires a priori knowledge of the viscoelastic properties of tissue, which is generally not the case. 
### Techniques

>[!NOTE] Rheometry
> - There are several standard techniques for characterising cavitation at lower strain rates including parallel plate, pulse-echo, and atomic force microscopy (AFM).
> - Higher strain rate rheology (>10 kHz) is performed using Kolsky Bar rheology which is not suited for heterogeneous, low-wave speed biomaterials.

> [!PDF|yellow] [[sreedasyam_2026_laser_cavitation_rheology.pdf#page=2&selection=52,18,57,34&color=yellow|sreedasyam_2026_laser_cavitation_rheology, p.2]]
> > The Split-Hopkinson (Kolsky) pressure bar remains the gold standard for high strain rate mechanical testing, but its reliance on stress wave propagation makes it poorly suited for spatially heterogeneous, low-wave speed biomaterials

![[sreedasyam_2026_laser_cavitation_rheology.pdf#page=2&rect=147,89,457,344|sreedasyam_2026_laser_cavitation_rheology, p.2]]

>[!NOTE] Cavitation rheology
> - There are several techniques that use cavitation to perform rheometry.
> - These span a range of strain rates, shear moduli, and size scales which makes the techniques flexible and widely applicable.
> - These techniques are applicable In Vivo to soft materials and biological tissues where standard techniques often fail.
> - Techniques include needle induced cavitation, laser induced cavitation, acoustic induced cavitation, and less common techniques such as shockwave-induced and confinement-induced cavitation.
> - Cavitation rheology most frequently uses high speed imaging to capture the bubble dynamics to characterise the material.
> - High speed imaging is not practical for widespread adoption in biomaterials and mechanobiology laboratories.
> - A new imaging technique needs to be developed for opaque materials.

> [!PDF|yellow] [[barney_2020_cavitation_in_soft_matter.pdf#page=3&selection=52,45,55,7&color=yellow|barney_2020_cavitation_in_soft_matter, p.3]]
> > Many of these techniques are focused toward soft materials and biological tissues, where standard techniques have issues with clamping, slip, and slump. 

> [!PDF|yellow] [[barney_2020_cavitation_in_soft_matter.pdf#page=3&selection=57,31,58,59&color=yellow|barney_2020_cavitation_in_soft_matter, p.3]]
> >  the unique capability of characterizing properties in the body offers significant promise 

> [!PDF|yellow] [[sreedasyam_2026_laser_cavitation_rheology.pdf#page=2&selection=122,3,135,69&color=yellow|sreedasyam_2026_laser_cavitation_rheology, p.2]]
> > While cavitation rheology represents a major advancement in the field, existing implementations are primarily designed to extract material properties at a single location by fitting the full bubble dynamics R(t), often using expensive and specialized ultra-high-speed videography hardware

> [!PDF|yellow] [[sreedasyam_2026_laser_cavitation_rheology.pdf#page=2&selection=138,15,146,7&color=yellow|sreedasyam_2026_laser_cavitation_rheology, p.2]]
> >  there remains a need for a cavitation rheology method that enables spatially resolved measurements of high strain rate material properties on the mesoscopic scale, using instrumentation that is practical for broad adoption by biomaterials and mechanobiology laboratories.
> 
> 

![[barney_2020_cavitation_in_soft_matter.pdf#page=5&rect=295,52,548,340&color=yellow|barney_2020_cavitation_in_soft_matter, p.5]]

>[!NOTE] Mapping bubble dynamics to local material properties
>- In cavitation rheology, the bubble dynamics must be connected with the properties of the material.
>- This is done using numerical simulations as the ground truth.

[find the quote for this]

---
# Research question

How can microbubbles and nonlinear imaging be used for microrheology for characterising viscoelastic properties of [collagen/fibrin/hydrogels/tissues].

- which soft tissues?
# Proposal

Microbubbles will be embedded in gels with known properties and subjected to nonlinear ultrasound imaging. Their response and acoustic emissions will be modelled [which models?] and various nonlinear imaging techniques [which ones?] will be assessed for their ability to produce measurable changes in the acoustic response of the microbubbles under a set of material parameters [under which material parameters?].

The acoustic emissions of the microbubbles will be measured using B-mode imaging and PCD and signal processing techniques [which ones?] will be used to estimate the properties of the medium. The B-mode data can be reconstructed after signal processing to obtain spatial information on the material properties. 

---
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