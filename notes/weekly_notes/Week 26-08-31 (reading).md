>[!TODO]
> - [ ] Read thesis by Rezaei
> - [ ] Check conclusions and future work
> - [ ] Find specific areas to focus on (imaging, signal processing, modelling)
> - [ ] Search for papers on NDs for microrheology

----
# Rezaei thesis

>[!ABSTRACT] Microbubbles in soft tissues
>- Analysis of how shifts in resonance frequency can measure changes in elastic modulus of the surrounding medium. 
>- Detecting shifts in resonance frequency using optical and acoustic methods.
>- Modelling coated microbubble dynamics in viscoelastic media.
>- Modelled the effect of a surrounding viscoelastic microcapillary.

- Combined effects of shell and medium viscoelasticity is unexplored.
> ([[rezaei_microbubble_acoustic_cavitation_soft_matter.pdf#page=43&selection=7,28,9,43&color=yellow|rezaei_microbubble_acoustic_cavitation_soft_matter, p.43]])
> the role of the combined effects of shell and medium viscoelasticity on the bubble dynamics and the consequences on the scattered ultrasound signals are still largely unexplored.

- Used simple Kelvin-Voigt for linear viscoelastic media.
> [[rezaei_microbubble_acoustic_cavitation_soft_matter.pdf#page=55&selection=9,0,11,14&color=yellow|rezaei_microbubble_acoustic_cavitation_soft_matter, p.55]]
> For simplicity, we used a Kelvin-Voigt linear viscoelastic model, which is valid for narrowband excitation, and as long as the medium remains within a linear deformation regime.

- Mentioned a statistical analysis of responses of a microbubble distribution as a potential avenue for future work.
> ([[rezaei_microbubble_acoustic_cavitation_soft_matter.pdf#page=55&selection=65,27,68,60&color=yellow|rezaei_microbubble_acoustic_cavitation_soft_matter, p.55]])
> A statistical analysis based on typical, or a range of size distributions of bubbles would provide insight into the nonlinear scattering of a suspension as compared to that of a single bubble, and thereby shed more light on the practical relevance of the results reported in this chapter.

- Mentioned nonlinear imaging as a potential avenue for future work.
> ([[rezaei_microbubble_acoustic_cavitation_soft_matter.pdf#page=55&selection=73,35,76,56&color=yellow|rezaei_microbubble_acoustic_cavitation_soft_matter, p.55]])
> The strong dependence of subharmonic scattering to the medium elasticity would furthermore allow for using nonlinear imaging, possibly using the TR to T2R ratio in order to measure the tissue elasticity with a high signal-to-background, or contrast-to-tissue, ratio.

> ([[rezaei_microbubble_acoustic_cavitation_soft_matter.pdf#page=75&selection=21,0,26,5&color=yellow|rezaei_microbubble_acoustic_cavitation_soft_matter, p.75]])
> Higher harmonics also bear interest, and can, in principle, be extracted from a Fourier filtering analysis. However, despite the narrow bandwidth of the transmitted pulses, the signal-to-noise ratio of the harmonic signal is too low to be able to reliably separate them from the fundamental spectrum. We suggest utilizing the pulse inversion (PI) technique to recover the nonlinear scattering in future investigations.

- Experimented with bubbles confined in viscoelastic microcapillaries.
> ([[rezaei_microbubble_acoustic_cavitation_soft_matter.pdf#page=79&selection=19,0,20,20&color=yellow|rezaei_microbubble_acoustic_cavitation_soft_matter, p.79]])
> Here, we experimentally investigate the dynamics of bubbles confined in viscoelastic microcapillaries

- Found that the bubbles should be driven at half their resonance frequency.
> ([[rezaei_microbubble_acoustic_cavitation_soft_matter.pdf#page=80&selection=6,0,9,40&color=yellow|rezaei_microbubble_acoustic_cavitation_soft_matter, p.80]])
> The frequency spectra of the radial dynamics show clear nonlinear second-harmonic oscillations when the bubble is driven at its resonance frequency and at half its resonance frequency. Notably, the latter is enhanced as compared to bubbles in the free field.

- First study to examine the effect of both the viscoelastic coating and media on bubble dynamics.
> ([[rezaei_microbubble_acoustic_cavitation_soft_matter.pdf#page=80&selection=13,43,15,13&color=yellow|rezaei_microbubble_acoustic_cavitation_soft_matter, p.80]])
> This is a unique study, as it examines both phospholipid coating and elastic microchannel effects in the regime of small oscillations.

>[!ABSTRACT] Modelling nonlinear scattering of microbubbles in a viscoelastic medium
>Modelled using a Kelvin-Voigt model to modify the Rayleigh-Plesset equation.

![[rezaei_modelling.pdf#page=2&rect=302,601,565,721|rezaei_modelling, p.2]]

- Found that the second harmonic was not significantly affected by the elastic modulus of the medium.
> ([[rezaei_modelling.pdf#page=6&selection=380,0,453,1&color=yellow|rezaei_modelling, p.6]])
> The amplitude 𝑃2𝐻 does not vary significantly with increasing elastic modulus, unlike the fundamental response. Specifically, the amplitude decreases by approximately 4% in a medium with 𝐺 = 200 kPa compared to 𝐺 = 0 kPa.

- Found that the second harmonic and fundamental were significantly affected.
> ([[rezaei_modelling.pdf#page=6&selection=1295,0,1338,1&color=yellow|rezaei_modelling, p.6]])
> The subharmonic scattered pressure generated by the bubble in the elastic material is approximately half that generated by the bubble in water.

----
# ADV for microrheology

### Microbubble dynamics in viscoelastic media

>[!ABSTRACT] Effect of medium stiffness on ADV dynamics
>Aliabouzar group has been examining the effect of medium stiffness on the dynamics of ADV using high-speed microscopy at 10 MHz.

- They found that the fibrin concentration did not significantly affect the initiation of ADV.
> [[abeid_ultra-high-speed_dynamics_of_adv_in_soft_biomaterials.pdf#page=4&selection=462,14,463,19&color=yellow|abeid_ultra-high-speed_dynamics_of_adv_in_soft_biomaterials, p.4]]
> Fibrin concentration did not significantly impact the initiation of ADV. 

- Factors that were most affected by fibrin concentration were:
> ([[abeid_ultra-high-speed_dynamics_of_adv_in_soft_biomaterials.pdf#page=4&selection=550,0,587,2&color=yellow|abeid_ultra-high-speed_dynamics_of_adv_in_soft_biomaterials, p.4]])
> The key parameters are as follows: maximum bubble radius (Rmax) at the peak time (t = tpeak), maximum expansion ratio (Λmax) defined as the ratio of an expanded bubble during ADV to the corresponding initial droplet radius (R0), the minimum bubble radius (Rc) during collapse, collapse time (tc) which is the time when the bubble reached its maximum size to its final collapse radius, rebound radius (Rreb), resting bubble radius at the end of high-speed microscopy at t = 20 μs (Rrest), and maximum expansion velocity (Vmax).

- They did not measure any parameters related to the ADV process itself.

### Numerical models of coated perfluorocarbon droplets in viscoelastic media

> [!ABSTRACT] Perfluorocarbon droplets with a viscoelastic shell in a viscoelastic fluid
> Gubaidullin developed a numerical model for perfluorocarbon droplets with a viscoelastic shell in a viscoelastic fluid. They assess the dynamic behaviour of the droplet but do not model the waves generated by the nanodroplet.

> ([[gubaidullin_2023_modelling_wave_dynamics_ADV.pdf#page=9&selection=12,0,14,56&color=yellow|gubaidullin_2023_modelling_wave_dynamics_ADV, p.9]])
> A system of differential equations that determines the radial oscillations of a vapor bubble inside an encapsulated perfluorocarbon droplet located in an external viscoelastic liquid under acoustic pressure action has been obtained.

![[gubaidullin_2023_modelling_wave_dynamics_ADV.pdf#page=3&rect=156,451,572,678&color=yellow|gubaidullin_2023_modelling_wave_dynamics_ADV, p.3]]

- They used the Kelvin-Voigt model for the viscoelastic shell and fluid.
> ([[gubaidullin_2023_modelling_wave_dynamics_ADV.pdf#page=4&selection=112,0,113,6&color=yellow|gubaidullin_2023_modelling_wave_dynamics_ADV, p.4]])
> For the carrier liquid and the shell of the droplet, we use the Kelvin–Voigt rheological model.

- In a later paper, they modelled nanodroplets in a viscoelastic medium with the Zener model.
> ([[gubaidullin_2024_acoustics_viscoelastic_liquid_droplets.pdf#page=2&selection=44,3,44,34&color=yellow|gubaidullin_2024_acoustics_viscoelastic_liquid_droplets, p.1989]])
> EQUATION OF RADIAL OSCILLATIONS

> ([[gubaidullin_2024_acoustics_viscoelastic_liquid_droplets.pdf#page=2&selection=500,32,501,79&color=yellow|gubaidullin_2024_acoustics_viscoelastic_liquid_droplets, p.1989]])
> The viscoelasticity of the carrier medium will be taken into account using the Zener rheological model

- Their model requires there to be a vapour phase inside the liquid nanodroplet to begin with.
> ([[gubaidullin_2024_acoustics_viscoelastic_liquid_droplets.pdf#page=2&selection=45,0,45,105&color=yellow|gubaidullin_2024_acoustics_viscoelastic_liquid_droplets, p.1989]])
> Let us consider a droplet of liquid with a vapor bubble at the center in an external viscoelastic liquid.

>[!ABSTRACT] Integrated model
> Zhao developed a model for ADV which integrates nucleation, growth, oscillation, and recondensation of nanodroplets.

> ([[zhao_2025_dynamics_ADV_dual_frequency.pdf#page=2&selection=9,54,29,11&color=yellow|zhao_2025_dynamics_ADV_dual_frequency, p.2]])
> Therefore, the primary objective of our work is to develop a unified, whole-process ADV model that integrates nucleation, growth and recondensation, and oscillation stages, while ensuring consistency in external environmental parameters.

- They use the Zener model for viscoelastic tissue.

> ([[zhao_2025_dynamics_ADV_dual_frequency.pdf#page=4&selection=724,0,725,6&color=yellow|zhao_2025_dynamics_ADV_dual_frequency, p.4]])
> Zener model has been used in this paper to simulate the viscoelastic tissue

### Machine learning for classifying medium properties

>[!ABSTRACT] PCD data, B-mode images, and transfer learning
> Aliabouzar group used PCD data and transfer learning to measure the fibrin density of their hydrogels. 

- They used features such as mean echo intensity, bubble cloud area measurements, and second-order texture features in the image.
> ([[kaushik_adv_tissue_characterisration_transfer_learning.pdf#page=3&selection=124,0,126,42&color=yellow|kaushik_adv_tissue_characterisration_transfer_learning, p.3]])
> Mean echo intensity was quantified, on log-decompressed images, by integrating pixel intensity values within a defined region of interest in each acquired frame.

> ([[kaushik_adv_tissue_characterisration_transfer_learning.pdf#page=3&selection=126,47,129,6&color=yellow|kaushik_adv_tissue_characterisration_transfer_learning, p.3]])
> area measurements, the threshold gray scale value separating the ADV bubble cloud from fibrin background was determined using Otsu’s method

> ([[kaushik_adv_tissue_characterisration_transfer_learning.pdf#page=4&selection=9,18,13,4&color=yellow|kaushik_adv_tissue_characterisration_transfer_learning, p.4]])
> In this study, four commonly reported GLCM parameters—contrast, variance, homogeneity, and energy— were calculated to describe various aspects of the texture, including pixel intensity relationships and overall texture uniformity.

- They used transfer learning (a machine learning algorithm designed to process images) on B-mode images and scalograms (unclear how these were generated) to characterise the fibrin concentrations and elastic modulus.
> ([[kaushik_adv_tissue_characterisration_transfer_learning.pdf#page=4&selection=221,32,224,19&color=yellow|kaushik_adv_tissue_characterisration_transfer_learning, p.4]])
> First, the input layer was adjusted to accommodate single-channel images (e.g., scalogram, B-mode, or CEUS mode images) by reducing the input channels from three to one. 

> ([[kaushik_adv_tissue_characterisration_transfer_learning.pdf#page=4&selection=228,21,230,49&color=yellow|kaushik_adv_tissue_characterisration_transfer_learning, p.4]])
> In addition, for BubbleNet2, the softmax layer was removed, allowing the model to perform regression tasks to predict elastic modulus values directly.

- They don't seem to quantify the signals from ADV itself. They are focused on the differences in the microbubbles formed by ADV.

> ([[kaushik_adv_tissue_characterisration_transfer_learning.pdf#page=3&selection=89,14,92,22&color=yellow|kaushik_adv_tissue_characterisration_transfer_learning, p.3]])
> To isolate and quantify vaporization signals generated from phase-shift droplets, B-mode and CEUS images were first acquired prior to transmitting the ADV pulse to capture the background signal.


----
# Microbubbles for microrheology

### Numerical models of microbubbles in a viscoelastic medium

>[!ABSTRACT] Microbubble interactions
>Qin developed a model for coated microbubbles in a viscoelastic medium with bubble-bubble interactions to assess the effect of microbubble and medium parameters on the cavitation threshold. 

![[qin_microbubble_interaction_dynamics.pdf#page=4&rect=163,494,568,714|qin_microbubble_interaction_dynamics, p.4]]

- They focused on inertial cavitation thresholds and used the Keller-Miksis equation with the Zener model for the viscoelastic shell and medium.

> ([[qin_microbubble_interaction_dynamics.pdf#page=4&selection=303,0,305,24&color=yellow|qin_microbubble_interaction_dynamics, p.4]])
> To describe the viscoelastic behaviors of the surrounding medium, the Zener model was used due to its superiority for describing the relaxation and elasticity behavior of soft tissues at the same time

- They modelled 2 bubbles at a time, investigating the effects of having differently-sized bubbles interacting.

> ([[qin_microbubble_interaction_dynamics.pdf#page=5&selection=583,10,585,7&color=yellow|qin_microbubble_interaction_dynamics, p.5]])
>  Model I and model II simulate two uncoated and two lipid-coated microbubbles oscillating in a soft tissue 

- Although their model is able to handle more than 2 microbubbles.
![[qin_microbubble_interaction_dynamics.pdf#page=3&rect=156,155,571,258&color=yellow|qin_microbubble_interaction_dynamics, p.3]]

----
### Future work

> [!question] Research Question
> How can we use microbubbles and nonlinear imaging for microrheology? 

>[!TODO] Modelling microbubbles
>- Model microbubble interactions in viscoelastic medium (see above).
>- Extract the signal generated by these microbubbles. 
>- Simulate nonlinear imaging modalities (e.g. pulse inversion, amplitude modulation, subharmonic imaging etc.)
>- Increase the number of microbubbles to assess the effect of bubble clouds on the spectral features.
>- Change the shear modulus of the material and look for measurable changes in spectral features (second and subharmonics).

>[!TODO] Signal processing
>- Develop signal processing pipeline to extract and classify medium properties based on RF data.
>- Develop beamforming algorithm on classified data to perform microrheology?
