You may use https://tex-image-link-generator.herokuapp.com/ to render math formulas in Markdown.

### PDEs

One mass balance per component water and CO2.

### Coupling of flow and transport, temporal and spatial discretization

Fully coupled, fully implicit, cell-centered FV with TPFA.

### Primary Variables

Dependent on local phase composition:
* Both phases present:
  ![p_l, S_g](https://render.githubusercontent.com/render/math?math=%5Ctextstyle+p_l%2C+S_g%0A)
* Only liquid phase present:
  ![p_l, x^{CO2}_l](https://render.githubusercontent.com/render/math?math=%5Ctextstyle+p_l%2C+x^{CO2}_l%0A)
* Only gas phase present:
  ![p_g, x^{H2O}_g](https://render.githubusercontent.com/render/math?math=%5Ctextstyle+p_g%2C+x^{H2O}_g%0A)

### Constitutive relations

#### Fluid-matrix interaction

* Capillary pressure: Brooks-Corey
  ![p_c(S_{l}) = p_\text{entry}S_{le}^{-1/\lambda}](https://render.githubusercontent.com/render/math?math=%5Cdisplaystyle+p_c%28S_%7Bl%7D%29+%3D+p_%5Ctext%7Bentry%7DS_%7Ble%7D%5E%7B-1%2F%5Clambda%7D%0A)
* Relative permeability: Brooks-Corey
  ![\begin{align*}
  k_{rl}(S_{l}) &= S_{le}^{2/\lambda + 3} \\
  k_{rg}(S_{l}) &= S_{ge}^2 (1.0 - S_{le}^{2/\lambda + 1})
  \end{align*}
  ](https://render.githubusercontent.com/render/math?math=%5Cdisplaystyle+%5Cbegin%7Balign%2A%7D%0Ak_%7Brl%7D%28S_%7Bl%7D%29+%26%3D+S_%7Ble%7D%5E%7B2%2F%5Clambda+%2B+3%7D+%5C%5C%0Ak_%7Brg%7D%28S_%7Bl%7D%29+%26%3D+S_%7Bge%7D%5E2+%281.0+-+S_%7Ble%7D%5E%7B2%2F%5Clambda+%2B+1%7D%29%0A%5Cend%7Balign%2A%7D%0A)

with ![S_{le}(S_l) = \frac{S_l - S_{lr}}{1 - S_{lr} - S_{gr}}, S_{ge} = 1 - S_{le}](https://render.githubusercontent.com/render/math?math=%5Cdisplaystyle+S_%7Ble%7D%28S_l%29+%3D+%5Cfrac%7BS_l+-+S_%7Blr%7D%7D%7B1+-+S_%7Blr%7D+-+S_%7Bgr%7D%7D%2C%0AS_%7Bge%7D+%3D+1+-+S_%7Ble%7D%0A)

The parameters ![p_\text{entry}, \lambda, S_{lr}, S_{gr}](https://render.githubusercontent.com/render/math?math=%5Cdisplaystyle+p_%5Ctext%7Bentry%7D%2C+%5Clambda%2C+S_%7Blr%7D%2C+S_%7Bgr%7D%0A)
for the different facies are given in [link to file]().

#### Dissolution and evaporation

* CO2 in liquid phase:

* Water in gas phase:

#### Density

* Liquid phase: 

* Gas phase: 
