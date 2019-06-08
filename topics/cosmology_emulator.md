# Cosmology Emulator

* Increasingly popular way to study cosmology based on a limit set of N-body simulations.

## Key Technique

* A suite of N-body cosmology simulations
	- 2nd order Lagrangian perturbation theory (2LPT) initial conditions
		* e.g. by [2LPTIC](http://cosmo.nyu.edu/roman/2LPT/) or on Github [here](https://github.com/manodeep/2LPTic)
	- Input power spectrum. e.g. by [CAMB: Code for Anisotropies in the Microwave Background](https://camb.info)

* Sampling the cosmological parameters:
	- Latin Hypercube Designs (LHDs)
	- [Maximin-distance “sliced” LHD (SLHD)](https://www.asc.ohio-state.edu/statistics/comp_exp/jour.club/optimal_sliced_lhd_ba2015.pdf)
    	- Python implementation: https://pythonhosted.org/pyDOE/index.html
    	- SMT: Surrogate Modeling Toolbox: https://smt.readthedocs.io/en/latest/index.html
    	- Another Python version: https://github.com/sahilm89/lhsmdu	

* Principle Component Analysis (PCA)
	- e.g. [empca](https://github.com/sbailey/empca) by Stephen Bailey

* Gaussian process emulator
	- e.g. [george](http://dfm.io/george/current/) by Dan Foreman-Mackey

## Available Emulators

- [Aemulus Project led by Stanford](https://aemulusproject.github.io)
	* The basic structure of the code: [Aemulator](https://github.com/AemulusProject/Aemulator)
	* Emulator of [halo mass function](https://github.com/AemulusProject/hmf_emulator) and [halo bias](https://github.com/AemulusProject/bias_emulator)
	* [The Aemulus Project I: Numerical Simulations for Precision Cosmology](https://arxiv.org/abs/1804.05865)
	* [The Aemulus Project II: Emulating the Halo Mass Function](https://arxiv.org/abs/1804.05866)
	* [The Aemulus Project III: Emulation of the Galaxy Correlation Function](https://arxiv.org/abs/1804.05867)
	* Documents for [data release 1](https://aemulus-data.readthedocs.io/en/latest/)
	
- [CosmicEmu led by ANL](http://www.hep.anl.gov/cosmology/CosmicEmu/emu.html)
	* Code can be found [here](https://github.com/lanl/CosmicEmu)
	* `CosmicEmu` produces predictions for the matter power spectrum based on eight cosmological parametersand redshift.
	* Based on the [Mira-Titan simulations](https://arxiv.org/abs/1508.02654)
	* Also related to the Coyote Universe emulator: [Paper I](https://arxiv.org/abs/0812.1052), [Paper II](https://arxiv.org/abs/0902.0429), [Paper III](https://arxiv.org/abs/0912.4490), and [Extended](https://arxiv.org/abs/1304.7849)
	* Paper about the [emulated power-spectrum](https://arxiv.org/abs/1311.6444)
	* Paper about the [emulated halo mass-concentration relation](https://arxiv.org/abs/1210.1576)
	
- [ACME Emulator led by OSU]()
	* Paper by Ben Wibking: [Emulating galaxy clustering and galaxy-galaxy lensing into the deeply nonlinear regime](http://adsabs.harvard.edu/doi/10.1093/mnras/sty2258)
	* Use the [AbacusCosmos suite of simulations](https://lgarrison.github.io/AbacusCosmos/)
		- The code used for the simulation is [here](https://github.com/lgarrison/AbacusCosmos)
		- The [AbacusCosmos description paper](https://arxiv.org/abs/1712.05768)
	
- [Dark Emulator led by IPMU]()
	* Based on the Dark Quest suite of simulations.
	* [Dark Quest. I. Fast and Accurate Emulation of Halo Clustering Statistics and Its Application to Galaxy Clustering](http://adsabs.harvard.edu/abs/2018arXiv181109504N)
	
