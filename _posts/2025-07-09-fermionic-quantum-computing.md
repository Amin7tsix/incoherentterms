---
title: "Fermionic Quantum Computing"
categories:
  - blog
tags:
  - Quantum computing
  - Paper summary
---

As is nowadays quoted in almost every introductory session on quantum computing, it was Feynman's dream/idea to simulate quantum behaviour with systems that themselves bahave quantum mechanically. Of course, everything is quantum mechanical at its core. However, what is meant here is observable and controllable quantum behaviour. 

<!--more-->

One of the most promising problems a quantum computer can help solve is to simulate molecular dynamics. There are many places you would want to do that. To calculate binding affinities in drug discovery, or to understand the catalysis of certain chemical reactions like nitrogen fixation. In these problems, the main task is usually 

Physical realizations of quantum computers are being pursued with different approaches, namely with superconducting circuits, trapped ions and trapped neutral atoms. Regardless of the technolgy, the common modality of processing quantum information which is pursued as of now is qubit based.


I recently came across this work:

https://www.pnas.org/doi/10.1073/pnas.2304294120

The authors discuss the idea of fermionic quantum computing. This can be seen in light of the famous Feynman's dream to simulate quantum behaviour using controllable "quantum" systems. The fermionic quantum computing idea is to use "fermionic" quantum systems to simulate "fermionic" quantum systems.

Here is the idea. The more common modality of a quantum computer is one based on a number of qubits and a

- normal: qubit based
- how simulate fermions with it?: mapping -> overhead
- now: fermion based
- why we need?: fermions have antisymmetry built in
- overhead is gone
- what makes it possible?: neutral atoms, in contrast with IR or microwave photons used in other QC realizations, can be fermion or boson. -> use fermionic atoms to hardwire fermionic statistics
- why exciting? can simulate fermionic systems: basically all chemistry/material science and biology are fermionic systems!
- how to implement? Electronic structure Hamiltonian (BO approx) -> 2-3 general operators enough -> Trotter -> implement one with shuttle/merge and another with Rydberg.
- catch: how about QEC? another paper discusses -> brings the overhead back (todo check this better)

$$
\hat{H}=\sum_{ij}h_{ij}\hat{c}^{\dagger}_i \hat{c}_j + \sum_{ijkl}g_{ijkl}\hat{c}^{\dagger}_i \hat{c}^{\dagger}_j \hat{c}_k  \hat{c}_l
$$

The paper is from 2023, but the idea goes back to earlier than that. Already in 2019, Bravyi and Kitaev showed that we can use