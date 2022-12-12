---
title: "High-quality Task Division for Large-scale Entity Alignment"
year: 2022
venue: 'CIKM 2022'
authors: [bing-liu, "Wen Hua", guido-zuccon, "Genghong Zhao", "Xia Zhang"]
pdf: https://arxiv.org/pdf/2208.10366.pdf
links:
 - url: https://github.com/uqbingliu/DivEA
   name: Code
---

## Abstract


Entity Alignment (EA) aims to match equivalent entities that refer to the same real-world objects and is a key step for Knowledge Graph (KG) fusion. Most neural EA models cannot be applied to large-scale real-life KGs due to their excessive consumption of GPU memory and time.
One promising solution is to divide a large EA task into several subtasks such that each subtask only needs to match two small subgraphs of the original KGs. However, it is challenging to divide the EA task without losing effectiveness. Existing methods display low coverage of potential mappings, insufficient evidence in context graphs, and largely differing subtask sizes.

In this work, we design the DivEA framework for large-scale EA with high-quality task division.
To include in the EA subtasks a high proportion of the potential mappings originally present in the large EA task, we devise a counterpart discovery method that exploits the locality principle of the EA task and the power of trained EA models. Unique to our counterpart discovery method is the explicit modelling of the chance of a potential mapping.
We also introduce an evidence passing mechanism to quantify the informativeness of context entities and find the most informative context graphs with flexible control of the subtask size.
Extensive experiments show that DivEA achieves higher EA  performance than alternative state-of-the-art solutions.