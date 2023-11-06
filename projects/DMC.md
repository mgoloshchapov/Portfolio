### Diffusion Monte Carlo

Diffusion Monte-Carlo is a useful tool for computing groundstate wavefunction and energy of quantum systems. [Here]() I implement basic version of DMC algorithm and give several examples of its work.

__Basic idea__

Suppose you want to find groundstate wavefunction and energy of a quantum system. If we replace time with imaginary time $t \rightarrow - i\tau$, arbitrary state will evolve as:

$$\left| \psi(\tau) \right>  = \sum_{n}c_n e^{- E_n \tau/ \hbar} \left| \psi_n \right>$$

We see that all summands decay exponentially. Now if we make energy shift equal to the ground state energy $E_0$, arbitrary state would evolve as

$$\left| \psi(\tau) \right>  =c_0 \left| \psi_0 \right>  + \sum_{n \neq 0}c_n e^{- (E_n-E_0) \tau/ \hbar} \left| \psi_n \right>,$$

so as $\tau \rightarrow \infty$ 

$$\left| \psi(\tau) \right> \rightarrow c_0 \left| \psi_0 \right> .$$

If initial projection of state on the ground state is not zero, we will eventually receive ground state of our system. By running algorithm with different energy shifts $E$ we can find one that doesn't grow/decay exponentially, which would correspond to ground state energy $E_0$.


<p align="center">
  <img src="{{site.url}}/images/DMC/harmonic.jpg" />
  <p align="center">
    Fig. 1: DMC groundstate for harmonic oscillator
  </p> 
</p>

<img src="{{site.url}}/images/dummy_thumbnail.jpg"/>

At each iteration of DMC the pligrims diffuse and implement birth/death step. Here is the visualization of pligrims lives in the double well potential and sampling of groundstate wavefunction.

<p align="middle">
  <img src="/projects/sources/dw_path_crop.gif" width="450"/>
  &nbsp; &nbsp; &nbsp; &nbsp;
  <img src="/projects/sources/dw_dmc.gif" width="450"/>

  <p align="center">
    Fig. 2: Left: Pligrims birth&death processes. Right: groundstate sampling.
  </p> 
</p>


Finally, DMC can be used to find groundstate of the Hydrogen atom:

<p align="middle">
  <img src="/projects/sources/hydrogen_invert.jpg" width="600"/>

  <p align="center">
    Fig. 3: Hydrogen atom groundstate radial part.
  </p> 
</p>

References:

[1] Ioan Kosztin et al., ["Introduction to the diffusion Monte-Carlo method"](https://arxiv.org/abs/physics/9702023v1)
