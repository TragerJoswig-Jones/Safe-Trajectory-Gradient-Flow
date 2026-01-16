# Safe-Trajectory-Gradient-Flow
This repository contains the code used to generate the results for the following paper: "[Safe Trajectory Gradient Flow Control of a Grid-Interfacing Inverter](https://arxiv.org/abs/2601.10671)"

Authors: Trager Joswig-Jones and Baosen Zhang  

University of Washington 

## Motivation
Grid-interfacing inverters allow renewable resources to be connected to the electric grid and offer fast and programmable control responses. However, inverters are subject to significant physical constraints. One such constraint is a current magnitude limit required to protect semiconductor devices. While many current limiting methods are available, they can often unpredictably alter the behavior of the inverter control during overcurrent events leading to instability or poor performance.

In this paper, we present a safe gradient flow based approach to iteratively optimize the predicted trajectory of a systems states, while maintaining a set of constraints on the states and inputs. A trajectory optimization problem is formulated and the trajectory is improved upon iteratively over a receding predicted horizon. The safe gradient flow approach allows for the trajectory to maintain anytime feasibility as a limited number of improving iterations are made in each time step. This approach, which we call ***Safe Trajectory Gradient Flow*** can be made less computationally expensive than model predictive control and can be implemented in real-time for systems that require fast control frequencies. We apply this approach to a grid-interfacing inverter control problem and demonstrate its capability to drive the system states to optimal points when given output power reference values that are infeasible due to the constraints on the inverters output current.

## Acknowledgments

The development of this code was supported in part by NSF grant ECCS-2023531.

The primary developer is Trager Joswig-Jones (joswitra@uw.edu).

This source code is available in the hope that it will be useful, but without any warranty and in no event shall the authors or copyright holders be liable for any claim, damages or other liability.

# Citing

If you find this repository useful in your work, we kindly request that you cite the following [publication](https://arxiv.org/abs/2601.10671):
```
@misc{joswigjones2026safetrajectorygradientflow,
      title={Safe Trajectory Gradient Flow Control of a Grid-Interfacing Inverter}, 
      author={Trager Joswig-Jones and Baosen Zhang},
      year={2026},
      eprint={2601.10671},
      archivePrefix={arXiv},
      primaryClass={eess.SY},
      url={https://arxiv.org/abs/2601.10671}, 
}
```
