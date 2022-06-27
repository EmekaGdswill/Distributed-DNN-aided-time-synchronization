# distributed-DNN-Aided-time-Synchronization Algorithm (DASA)
This is the Python repository for the paper ["Deep Learning Aided Distributed Clock Synchronization for Wireless Networks"](http://arxiv.org/abs/2206.12097)\
The code obtains network clock synchronization for wireless sensor nodes via pulse coupled PLLs at the nodes\
Please cite our paper, if the code is used for publishing research.


The widely studied classic physical layer synchronization scheme based on the update rule ([see link](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=4607217)) is known to fail in achieving full synchronization  for networks with non-negligible  propagation delays, and/or the clock frequency differences among the nodes, resulting in clusters of nodes synchronized among themselves, while the clocks of nodes belonging to different clusters are not phase-synchronized.
In this work, we design an algorithm, abbreviated as DASA, which replaces the analytically computed $a_{ij}$ coefficients  of the classic algorithm 	with weights learned  using \acp{dnn}, such that learning is done  in an  unsupervised and distributed manner, and requires a very short training period. These properties make the proposed algorithm very attractive for practical implementation. With the proposed DASA scheme, each node determines its subsequent clock phase using its own clock and the timings of the pulses received from the other nodes in the network. \
Our results show that when there are propagation delays and clock frequency differences between the nodes, both the proposed \ac{dasa} and the classic analytically-based scheme achieve frequency synchronization, however only the DASA is able to attain full synchronization of both the frequency and phase with a very high  accuracy.
