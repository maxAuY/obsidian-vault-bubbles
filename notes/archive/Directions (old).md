--- classifying cavitation ---
- classify stable and transient
	- machine learning wavelet transform project
- classify activated/non-activated
	- activation is usually measured using optical methods (see monitoring adv folder)
	- increase in fundamental and sub-harmonics for activated NDs
	- ADV may be counterproductive with high pressures (ovenden: non-equilibrium vaporisation dynamics of superheated phase-change contrast agents)
	- standardised adv definition (oberhuber: Impact of perfluorocarbon nanodroplet fabrication and ADV)
	- are non-activated NDs visible?
	- short-term project useful for understanding experimental results?
	- could be a longer-term project involving estimating the percentage of activated NDs from subharmonic emissions.
	- could include broadband and harmonics as features for classification.
	- will have to image to calculate percentage activation?
- classify NDs inside and outside cells
	- problem is that resolution is not high enough, cannot see single bubbles
	- nondestructive methods are required. destruction-replenishment is slow and could damage tissue.
	- umi methods can take advantage of temporal differences (movement) or non-linearity (higher non-linearity from bubbles).
	- see collado-lara non-destructive paper
	- estimate the resolution achievable by the methods
- quantification of cell concentration
	- use inside/outside classification to extract signals from cells
	- find correlation between cell concentration and pixel intensity

--- improved background removal ---
* removing linear background
	* most of the field has not yet moved on from amplitude modulation (and pulse inversion etc.)
	* cross amplitude modulation (david maresca) is the standard for GVs
	* chirp signals and volterra filtering could be used to enhance and extract nonlinear signals
* removing non-linear background
	* tissues can have non-linear oscillations. these cannot be easily removed using  harmonic imaging.
	* many approaches just note an increase in non-linearity and do not fully remove background.
	* might be possible to calculate expected non-linear propagation and subtract?
	* train an AI to recognise nonlinear signals from tissue?
	* what is the application?
* improved beamforming techniques
	* TODO

--- tasks ---
* optimise activation pulse
	* develop percentage activation measurement
	* optimise activation pulse based off of this measurement
* background removal with non-linear imaging pulse
	* model with scattering + nonlinear signal generation with coated bubbles
	* simulate non-linear imaging with low sampling rate
	* if it is, can we predict what the pulse will be and cancel it with a new algorithm instead of using harmonic imaging?
* wavelet transform and machine learning
	* machine learning for better clustering, improving on aliasing effects
* active cavitation detection (wavelet transform + k-means)
	* extension of existing paper
* beamforming with wavelet transform (simulation)
	* coated bubble dynamics
	* radiated pressure
	* simulated array
	* k-means on all elements