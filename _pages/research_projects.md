---
layout: page
permalink: /Projects/
title: Projects
description: Ongoing Research Projects 
nav: true
nav_order: 3
---
<div style="font-weight: bold; font-size: 1.5em; margin-top: 20px; margin-bottom: 10px;"> Belief Propagation with Quantum Messages over CQ Channels</div>
<hr style="border: 1px solid #ccc; margin-bottom: 15px;">
Belief propagation (BP) is a classical algorithm that approximates the marginal distribution associated with a factor graph by passing messages between adjacent nodes. <br>
In 2016, Renes developed belief propagation with quantum messages <a href="https://iopscience.iop.org/article/10.1088/1367-2630/aa7c78/pdf">(BPQM) </a> and described how it could be used to decode classical codes defined by tree factor graphs that are sent over the classical-quantum pure-state channel.<br>
<div style="display: flex; align-items: center;">
  <p style="margin-right: 10px;">

In this research, we extend the classical belief propagation algorithm to a method called Paired Measurement Belief Propagation with Quantum Messages (PM-BPQM) for binary symmetric classical-quantum (BSCQ) channels. A tree factor graph based classical code can be analyzed using two channel combining operations- check-node and bit-node combining. We obtained sufficient statistics based on classical parameters for channel combining operations (check-node and bit-node combining) for quantum states from CQ channel outputs via PM-BPQM. Using these classical parameters and monte carlo based density evolution, we characterized the asymptotic performance (e.g. finding noise thresholds) of tree based codes (regular low-denisty parity-check (LDPC), polar codes) over BSCQ channels.
<br> We deveoped PM-BPQM based polar decoder over BSCQ channels and provided its performance.
 </p>
  <img src="../assets/img/polar_bpqm.gif" alt="BPQM based CQ Polar Decoding" width="300">
</div>
<br> Here are the list of papers which gives more insight on this topic
1. Belief propagation with quantum messages for symmetric classical-quantum channels, <a href="https://ieeexplore.ieee.org/abstract/document/9965841"> ITW 2022</a> <a href="https://arxiv.org/abs/2207.04984"> (arxiv version)</a><br> 
2. Belief-propagation with quantum messages for polar codes on classical-quantum channels, <a href="https://ieeexplore.ieee.org/abstract/document/10206723"> ISIT 2023 </a> <br>
3. Polar Codes for CQ Channels: Decoding via Belief-Propagation with Quantum Messages <a href="https://arxiv.org/pdf/2401.07167"> (arxiv preprint) </a>. 

<br> Here are the relevant repositories 
1. Finding thresholds for regular LPDC codes over BSCQ channels - <a href="https://github.com/Aviemathelec1995/PMBPQM_BSCQ"> PMBPQM_BSCQ </a>
2. Simulating Polar Decoder over BSCQ channels - <a href="https://github.com/Aviemathelec1995/CQ-Polar-BPQM"> CQ-Polar-BPQM </a>.

<div style="font-weight: bold; font-size: 1.5em; margin-top: 20px; margin-bottom: 10px;"> Quantum State Compression with Polar Codes</div>
<hr style="border: 1px solid #ccc; margin-bottom: 15px;">
In Quantum State Compression poblem, Alice wants to transmit her quantum states to Bob using the least number of qubits possible.<br>
In 1995, Schumacher proposed the first method for rate-optimal lossless quantum state compression and it can be seen as a generalization of Shannon’s original protocol for rate-optimal lossless classical compression. However, direct implementation on a quantum computer is quite complex.<br>
The idea of syndrome source coding was first introduced in 1976 by Ancheta which provides an approach to use linear codes for classical compression problems.The complexity of syndrome source coding can be reduced if linear codes used for the compression have low encoding and decoding complexity. Polar codes are also known to be rate-optimal for lossless compression problems.<br>
In this work, we develop a belief propagation (BP) based low complexity quantum state compressor and decompressor using polar codes. For quantum state decompressor, we treat frozen bits of polar codes as syndrome qubits and information bits are kept as ancilla. Using BP we construct conditional unitary which determines the state of information qubits coherently. Thus we get coherent version of polar source coding protocol based on BP. The quantum state compressor follows the same principle as the decompressor.<br>

The published version of this work can be found here- Quantum State Compression with Polar Codes <a href="https://ieeexplore.ieee.org/document/10619556"> ISIT 2024 </a>.

The code repository can be found here - <a href="https://github.com/Aviemathelec1995/QSCpolar"> QSCPolar</a>.
