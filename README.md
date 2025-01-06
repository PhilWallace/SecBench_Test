# SecBench: A Comprehensive Multi-Dimensional Benchmarking Dataset for LLMs in Cybersecurity

Evaluating Large Language Models (LLMs) is crucial for understanding their capabilities and limitations across various applications, including natural language processing and code generation. Existing benchmarks like MMLU, C-Eval, and HumanEval assess general LLM performance but lack focus on specific expert domains such as cybersecurity. Previous attempts to create cybersecurity datasets have faced limitations, including insufficient data volume and a reliance on multiple-choice questions (MCQs). To address these gaps, we propose SecBench, a multi-dimensional benchmarking dataset designed to evaluate LLMs in the cybersecurity domain. SecBench includes questions in various formats (MCQs and short-answer questions (SAQs)), at different capability levels (Knowledge Retention and Logical Reasoning), in multiple languages (Chinese and English), and across various sub-domains. The dataset was constructed by collecting high-quality data from open sources and organizing a Cybersecurity Question Design Contest, resulting in 44,823 MCQs and 3,087 SAQs. Particularly, we used the powerful while cost-effective LLMs to (1). label the data and (2). constructing a grading agent for automatic evaluation of SAQs. Benchmarking results on 16 SOTA LLMs demonstrate the usability of SecBench, which is arguably the largest and most comprehensive benchmark dataset for LLMs in cybersecurity.


SecBench official website: *[link](https://secbench.org/)*.

SecBench Technical Paper: *[link](https://arxiv.org/abs/2412.20787)*.


## SecBench Design






## Benchmarking


| #   | Model             | Creator   | Access    | Submission Date | System Security | Application Security | PenTest | Memory Safety | Network Security | Web Security | Vulnerability | Software Security | Cryptography | Overall |
|-----|-------------------|-----------|-----------|-----------------|-----------------|----------------------|---------|---------------|------------------|--------------|---------------|-------------------|--------------|---------|
| 1   | gpt-4-turbo       | OpenAI    | API, Web  | 2023-12-20      | 73.61           | 75.25                | 80.00   | 70.83         | 75.65            | 82.15        | 76.05         | 73.28             | 64.29        | 79.07   |
| 2   | gpt-3.5-turbo     | OpenAI    | API, Web  | 2023-12-20      | 59.15           | 57.18                | 72.00   | 43.75         | 60.87            | 63.00        | 60.18         | 58.19             | 35.71        | 62.09   |
| 3   | Yi-6B             | 01-AI     | Weight    | 2023-12-20      | 50.61           | 48.89                | 69.26   | 35.42         | 56.52            | 54.98        | 49.40         | 45.69             | 35.71        | 53.57   |
| 4   | Orca-2-7b         | Microsoft | Weight    | 2023-12-20      | 46.76           | 47.03                | 60.84   | 31.25         | 49.13            | 55.63        | 50.00         | 52.16             | 14.29        | 51.60   |
| 5   | Mistral-7B-v0.1   | Mistralai | Weight    | 2023-12-20      | 40.19           | 38.37                | 53.47   | 33.33         | 36.52            | 46.57        | 42.22         | 43.10             | 28.57        | 43.65   |
| 6   | chatglm3-6b-base  | THUDM     | Weight    | 2023-12-20      | 39.72           | 37.25                | 57.47   | 31.25         | 43.04            | 41.14        | 37.43         | 39.66             | 28.57        | 41.58   |
| 7   | Aquila2-7B        | BAAI      | Weight    | 2023-12-20      | 34.84           | 36.01                | 47.16   | 22.92         | 32.17            | 42.04        | 38.02         | 36.21             | 7.14         | 38.29   |
| 8   | Qwen-7B           | Alibaba   | Weight    | 2023-12-20      | 28.92           | 28.84                | 41.47   | 18.75         | 29.57            | 33.25        | 31.74         | 30.17             | 14.29        | 31.37   |
| 9   | internlm-7b       | Sensetime | Weight    | 2023-12-20      | 25.92           | 25.87                | 36.21   | 25.00         | 27.83            | 32.86        | 29.34         | 34.05             | 7.14         | 30.29   |
| 10  | Llama-2-7b-hf     | MetaAI    | Weight    | 2023-12-20      | 20.94           | 18.69                | 26.11   | 16.67         | 14.35            | 22.77        | 21.56         | 20.26             | 21.43        | 22.15   |

 - **fuzzing** : The improved fuzzing framework, refined with the range restriction mutation, and the improved fitness score constructed from new metrics.

 - **refined_mpc_controller** : The refined controller code, which outperforms the original controller after we fixed identified bugs.

 - **oracle_assessment** : How to assess the controller performance based on the proposed four metrics.

 - **VLM_Results** : The results produced by GPT-4o VLM in our CoT based bug analysis.




## Citation


```bibtex
@article{jing2024secbench,
  title={SecBench: A Comprehensive Multi-Dimensional Benchmarking Dataset for LLMs in Cybersecurity},
  author={Jing, Pengfei and Tang, Mengyun and Shi, Xiaorong and Zheng, Xing and Nie, Sen and Wu, Shi and Yang, Yong and Luo, Xiapu},
  journal={arXiv preprint arXiv:2412.20787},
  year={2024}
}3}
}
```