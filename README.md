Today, as embedded devices' computational ability increases, more and more Deep Neural Networks~(DNNs) have been deployed on embedded devices to assist in systems' decision making.
However, directly running DNNs on resource-constrained embedded devices can not meet system requirements~(e.g., real-time prediction, energy efficiency).
To address this challenge, researchers propose a series of Adaptive Neural Networks~(AdNNs). However, because AdNNs adapt to optimal computation resource allocation on a given input, AdNNs can still have performance degradation issues on some inputs.
Such AdNNs performance degradation depends on the input workloads, referred to as input-dependent performance bottlenecks (IDPBs). To ensure an AdNN keeping the expected performance after deployment, it is important to conduct performance testing to detect  IDPBs in the AdNN. To the best of our knowledge, most testing methods for Neural Networks are focused on correctness testing, which does not involve detecting IDPBs.
To fill this gap, we propose a performance testing framework that could generate test samples to detect the IDPB of AdNNs.
Specifically, we propose DeepPerform,  an efficient performance testing framework against a common type of AdNNs.
We first leverage the idea of metamorphic testing to detect the IDPB automatically.
Next, we demonstrate how the problem of generating performance test samples detecting IPDBs can be formulated as an optimization problem.
Finally, we show how DeepPerform could solve the optimization problem efficiently through learning and approximating the distribution of AdNNs computation consumption.
Once DeepPerform is trained, DeepPerform can efficiently generate test samples to trigger IDPB for any seed image, so as to benefit the performance testing process.
