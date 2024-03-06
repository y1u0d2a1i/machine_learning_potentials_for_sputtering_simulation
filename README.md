# Machine learning interatomic potentials of Si for sputtering simulation


# Repository Description

This repository contains a machine learning interatomic potential for Silicon (Si), developed for sputtering simulation as part of the research outlined below. The `models` directory houses several machine learning potentials, named from `model1` to `model5`.

## Models Directory Structure

Each `model` directory includes four files essential for the machine learning model's operation. The table below provides a description for each file type:

| File Name          | Description                                         |
|--------------------|-----------------------------------------------------|
| `input.data`       | The training data.                                  |
| `input.nn`         | The training configuration file.                    |
| `scaling.data`     | Data necessary for normalizing the data within n2p2.|
| `weights.014.data` | Neural network weights file.                        |

## Model Descriptions

The specifics for models `model1` through `model5` are as detailed in the associated paper, corresponding to different configurations of amorphous Silicon and dimer formations:

- `model1`: Amorphous: 0
- `model2`: Amorphous: 676
- `model3`: Amorphous: 6154
- `model4`: Amorphous: 11983
- `model5`: Amorphous: 11983, Dimer: 800

For further details on these models, please refer to the published paper.

## Versions of Software Used
We utilized n2p2[1] for the creation of the machine learning interatomic potentials. The sputtering simulations were conducted in LAMMPS[2], through the interface provided by n2p2[3]. Below are the versions of n2p2 and LAMMPS we used:

| Software | Version |
|----------|---------|
| n2p2     | v2.1.4   |
| LAMMPS   | 2 Aug 2023 - Update 1    |

<br>
[1] Singraber, A.; Morawietz, T.; Behler, J.; Dellago, C. Parallel Multistream Training of High-Dimensional Neural Network Potentials. J. Chem. Theory Comput. 2019, 15 (5), 3075–3092.
[2] LAMMPS - a flexible simulation tool for particle-based materials modeling at the atomic, meso, and continuum scales, A. P. Thompson, H. M. Aktulga, R. Berger, D. S. Bolintineanu, W. M. Brown, P. S. Crozier, P. J. in 't Veld, A. Kohlmeyer, S. G. Moore, T. D. Nguyen, R. Shan, M. J. Stevens, J. Tranchida, C. Trott, S. J. Plimpton, Comp Phys Comm, 271 (2022) 10817.
[3] Singraber, A.; Behler, J.; Dellago, C. Library-Based LAMMPS Implementation of High-Dimensional Neural Network Potentials. J. Chem. Theory Comput. 2019, 15 (3), 1827–1840.