# MoMQ: Mixture-of-Experts Enhances Multi-Dialect Query Generation across Relational and Non-Relational Databases


## News🔥
We will be releasing code related to MoMQ, an advanced multi-dialect SQL MOE model.


## Overview
![](momq_pipeline.png.png)



## Introduction
The improvement in translating natural language to structured query language (SQL) can be attributed to the advancements in large language models (LLMs). Open-source LLMs, tailored for
specific database dialects such as MySQL, have shown great performance. However, cloud service providers are looking for a unified database manager service (e.g., Cosmos DB from Azure, Amazon Aurora from AWS, Lindorm from AlibabaCloud) that can support multiple dialects. This requirement has led to the concept of multidialect query generation, which presents challenges to LLMs. These challenges include syntactic differences among dialects and imbalanced data distribution across multiple dialects. To tackle these challenges, we propose MoMQ, a novel Mixture-of-Experts-based multi-dialect query generation framework across both relational and non-relational databases. MoMQ employs a dialect expert group
for each dialect and a multi-level routing strategy to handle dialectspecific knowledge, reducing interference during query generation. Additionally, a shared expert group is introduced to address data imbalance, facilitating the transfer of common knowledge from high-resource dialects to low-resource ones. Furthermore, we have
developed a high-quality multi-dialect query generation benchmark that covers relational and non-relational databases such as MySQL, PostgreSQL, Cypher for Neo4j, and nGQL for NebulaGraph. Extensive experiments have shown that MoMQ performs effectively and robustly even in resource-imbalanced scenarios.




## Citation
If you find our work helpful, feel free to give us a cite.
```bibtex
@article{momq_sql,
      title={MoMQ: Mixture-of-Experts Enhances Multi-Dialect Query Generation across Relational and Non-Relational Databases}, 
      author={Zhisheng Lin and Yifu Liu and Zhiling Luo and Jinyang Gao and Yu Li},
      year={2024},
      journal={arXiv preprint arXiv:2410.18406},
      url={https://arxiv.org/abs/2410.18406},
      primaryClass={cs.CL},
}
```
