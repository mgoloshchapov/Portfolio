### Domain wall pinning & Magnetic memory in Ising model.

What happens with spin configurations in Ising model if we add impurities?

<p align="middle">
  <img src="./images/pinning.jpg"/>

  <p align="center">
    Fig. 1: Spin-zero impurities on 2D lattice.
  </p> 
</p>

We receive domain wall pinning!

<p align="middle">
  <img src="./images/cells.jpg"/>

  <p align="center">
    Fig. 2: Domain walls pin to impurities and form square cells.
  </p> 
</p>

By estimating correlation length for spins we can adjust square cell size formed by impurities 
to reduce correlations between adjacent cells, so Monte-Carlo sweeps don't change cell magnetization.

<p align="middle">
  <img src="./images/radius.jpg"/>

  <p align="center">
    Fig. 3: Circles with radius equal to correlation length received from autocorrelation function. 
            Correlation length is a good estimate for domain thickness.
  </p> 
</p>

Now if we start applying local magnetic field to individual cells,
we can change magnetization of the whole cell. 
This corresponds to writing information in it. 

Due to the educated choice of 
square cell size, adjacent cells almost don't interact with each other, so information can be stored inside them.

<p align="middle">
  <img src="./images/memory.gif"/>

  <p align="center">
    Fig. 4: Local magnetic field changes magnetization of cells. Monte-Carlo sweeps don't change magnetization of cells.
  </p> 
</p>
