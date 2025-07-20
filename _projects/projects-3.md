---
title: "MAE-DFER-CA"
excerpt: "Efficient self-supervised dynamic facial emotion recognition, integrating channel attention into MAE-DFER for improved accuracy and reduced computational cost.<br/><a href='https://github.com/drink36/MAE-DFER-CA'><img src='/images/Model.png' style='width:350px; border-radius:12px; box-shadow:0 2px 10px rgba(0,0,0,.1);'></a><br/><span style='font-size:90%;color:#888;'>Overview of MAE-DFER-CA</span>"
collection: projects
---

**MAE-DFER-CA** extends the masked autoencoder framework for dynamic facial expression recognition (DFER) by integrating a Channel Attention (CA) module to enhance subtle muscle motion pattern learning. This work builds upon the MAE-DFER architecture, which employs the LGI-Former encoder for efficient self-supervised video representation.

**Key Features:**
- Self-supervised masked autoencoder based on MAE-DFER, reducing annotation dependence for dynamic facial emotion recognition.

- Integrates channel attention (CA_Module, inspired by MMNET) to enhance subtle motion pattern learning between video frames.

- Achieves stable accuracy gains (WAR 52.40 on FERV39k) with only a minimal increase in computational cost (FLOPs).

- Validated consistent improvement over the original MAE-DFER on real-world benchmark datasets.


**System Overview**

![Overview of MAE-DFER-CA](/images/Model.png)
<p align="center"><span style="font-size:90%;color:#888;">Overview of the MAE-DFER framework with integrated Channel Attention module.</span> </p>
The framework models both spatial and temporal features by combining joint masked appearance and motion reconstruction with channel attention, enabling improved recognition of subtle, dynamic facial expressions in video sequences.

![Channel Attention Module](/images/CA_Module.png)
<p align="center"><span style="font-size:90%;color:#888;">Architecture of the Channel Attention (CA) module, adapted from micro-expression recognition techniques.</span> </p>

![Performance on FERV39k](/images/Result_on_FERV39k.png)
<p align="center"><span style="font-size:90%;color:#888;">Performance comparison on the FERV39k dataset, highlighting the consistent gain from the Channel Attention integration.</span> </p>

[View on GitHub](https://github.com/drink36/MAE-DFER-CA){: .btn .btn--primary }