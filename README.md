# Modeling Stellar Clusters Using COMPAS
This repository provides input and output data from three COMPAS simulation sets evolving cluster-like populations from Gaia DR2 and DR3.

## File Summary
| File Name            | Description                                                |
| -------------------- | ---------------------------------------------------------- |
| `README.md`          | This file                                                  |
| `DR2_1_clusters.csv` | Physical parameters for 387 simulated clusters, DR2(1) run |
| `DR2_2_clusters.csv` | Physical parameters for 387 simulated clusters, DR2(2) run |
| `DR3_clusters.csv`   | Physical parameters for 215 simulated clusters, DR3 run    |
| `DR2_2_sampled.csv`  | Semi-major axes, M1, and M2 of cluster members, DR2(2) run |
| `DR3_sampled.csv`    | Semi-major axes, M1, and M2 of cluster members, DR3 run    |

---

## File Descriptions

### `DR2_1_clusters.csv`, `DR2_2_clusters.csv`, `DR3_clusters.csv`
| Units   | Label     | Description                                                |
| ------- | --------- | ---------------------------------------------------------- |
| ---     | `Cluster` | Cluster name                                               |
| Myr     | `Age`     | Cluster age [1]                                            |
| ---     | `k`       | Normalization of the initial mass function [1][4]          |
| ---     | `N`       | Number of stars in cluster                                 |
| ---     | `Nsys`    | Number of simulated binary systems                         |
| ---     | `Z`       | Metallicity [2][3]                                         |
| ---     | `bin_frac` | Binary fraction [3]                                       |
| AU      | `a`       | Initial semi-major axis                                    |
| M☉      | `Mc`      | Cluster mass                                               |
| M☉ yr⁻¹ | `Mdot`    | Cluster wind mass-loss rate                                |
| W       | `Lw`      | Cluster wind luminosity                                    |
| ---     | `SNe`     | Number of supernovae                                       |
| ---     | `WR`      | Number of WR stars, based on dominant mass-loss rate       |
| ---     | `WR2`     | Number of WR stars, based on stellar mass and stellar type |

### `DR2_2_sampled.csv`, `DR3_sampled.csv`
| Units | Label | Description                     |
| ----- | ----- | ------------------------------- |
| AU    | `a`   | Initial semi-major axis         |
| M☉    | `M1`  | Initial mass of primary stars   |
| M☉    | `M2`  | Initial mass of secondary stars |

---

## Notes
* Quantities `Mc`, `Mdot`, `Lw`, `SNe`, `WR`, and `WR2` have been multiplied by a factor of 5 to scale from the simulated population (20% of cluster members) to the estimated full cluster population.

---

## References
[1] Celli et al. (2024), *Mass and wind luminosity of young Galactic open clusters in Gaia DR2*
https://doi.org/10.1051/0004-6361/202348541

[2] Kharchenko et al. (2013), *Global survey of star clusters in the Milky Way. II. The catalogue of basic parameters*
https://doi.org/10.1051/0004-6361/201322302

[3] Almeida et al. (2023), *Revisiting the mass of open clusters with Gaia data*
https://doi.org/10.1093/mnras/stad2291

[4] Hunt et al. (2024), *Improving the open cluster census: III. Using cluster masses, radii, and dynamics to create a cleaned open cluster catalogue*
https://doi.org/10.1051/0004-6361/202348662
