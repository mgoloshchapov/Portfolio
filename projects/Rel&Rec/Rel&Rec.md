### Release & Recapture - Atom Temperature

Temperature of single atom in optical tweezers can be measured via release & recapture experiment. 
The basic idea of this experiment is to turn off the dipole trap and measure probability to recapture atom after variable release time.
If the atom is hot, it will quickly escape the trap, so recapture probability will decay fast. If the atom is cold, it will stay in the trap longer, so recapture probability will decay slower. By fitting experimental data from release&recapture experiment with Monte-Carlo simulation, we can extract atom's temperature.

<p align="middle">
  <img src="./images/temperature.pdf"/>

  <p align="center">
    Fig. 1: Recapture probability decay from release time, Monte-Carlo fit.
  </p> 
</p>

Metropolis-Hastings algorithm is used to obtain samples of coordinates and velocities for atom in the dipole trap. 

<p align="middle">
  <img src="./images/samples.pdf"/>

  <p align="center">
    Fig. 2: Coordinate and velocity distributions for atom in deep trap. 
  </p> 
</p>

