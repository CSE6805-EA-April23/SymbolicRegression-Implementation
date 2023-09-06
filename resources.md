# Problem Formulation
A generalization of the concept of linear regression or polynomial regression is to try to search over the space of all possible mathematical formulas for the ones that best predict the output variable, taking as input the input variables, starting from a set of base functions like addition, trigonometric functions, and exponentials. This is the basic idea of symbolic regression.

## High level optimization goals
- Discard a large formula if a smaller one with the same accuracy is encountered.
- Make solutions more Interpretable to the human eye.
- Maximize accuracy.

# Relevant Literature
***to be added***


# Benchmarked Methods

This benchmark currently consists of **14** symbolic regression methods, **7** other ML methods, and **252** datasets from [PMLB](https://github.com/EpistasisLab/penn-ml-benchmarks), including real-world and synthetic datasets from processes with and without ground-truth models.

Methods currently benchmarked:

- Age-Fitness Pareto Optimization (Schmidt and Lipson 2009) 
    [paper](https://dl.acm.org/doi/pdf/10.1145/1830483.1830584)
    , 
    [code](https://github.com/cavalab/ellyn)
- Age-Fitness Pareto Optimization with Co-evolved Fitness Predictors (Schmidt and Lipson 2009) 
    [paper](https://dl.acm.org/doi/pdf/10.1145/1830483.1830584?casa_token=8fAFUrPlfuUAAAAA:u0QJvX-cC8rPtdZri-Jd4ZxcnRSIF_Fu2Vn5n-oXVNu_i71J6ZECx28ucLPOLQY628drsEbg4aFvTw)
    , 
    [code](https://github.com/cavalab/ellyn)
- AIFeynman 2.0 (Udrescu et al. 2020)
    [paper](https://arxiv.org/abs/2006.10782)
    ,
    [code](https://github.com/SJ001/AI-Feynman)
- Bayesian Symbolic Regression (Jin et al. 2020)
    [paper](https://arxiv.org/abs/1910.08892)
    ,
    [code](https://github.com/ying531/MCMC-SymReg)
- Deep Symbolic Regression (Petersen et al. 2020)
    [paper](https://arxiv.org/pdf/1912.04871)
    , 
    [code](https://github.com/brendenpetersen/deep-symbolic-optimization)
- Fast Function Extraction (McConaghy 2011)
    [paper](http://trent.st/content/2011-GPTP-FFX-paper.pdf)
    ,
    [code](https://github.com/natekupp/ffx)
- Feature Engineering Automation Tool (La Cava et al. 2017)
    [paper](https://arxiv.org/abs/1807.00981)
    ,
    [code](https://github.com/lacava/feat)
- epsilon-Lexicase Selection (La Cava et al. 2016)
    [paper](https://arxiv.org/abs/1905.13266)
    ,
    [code](https://github.com/cavalab/ellyn)
- GP-based Gene-pool Optimal Mixing Evolutionary Algorithm (Virgolin et al. 2017)
    [paper](https://dl.acm.org/doi/pdf/10.1145/3071178.3071287?casa_token=CHa8EK_ic5gAAAAA:mOAOCu6CL-jHobGWKD2wco4NbpCyS-XTY5thb1dPPsyUkTkLHzmLMF41MWMGWLyFv1G8n-VFaqmXSw)
    ,
    [code](https://github.com/marcovirgolin/GP-GOMEA/)
- gplearn (Stephens)
    [code](https://github.com/trevorstephens/gplearn)
- Interaction-Transformation Evolutionary Algorithm (de Franca and Aldeia, 2020)
    [paper](https://www.mitpressjournals.org/doi/abs/10.1162/evco_a_00285)
    ,
    [code](https://github.com/folivetti/ITEA/)
- Multiple Regression GP (Arnaldo et al. 2014)
    [paper](https://dl.acm.org/doi/pdf/10.1145/2576768.2598291?casa_token=Oh2e7jDBgl0AAAAA:YmYJhFniOrU0yIhsqrHGzUN_60veH56tfwizre94uImDpYyp9RcadUyv_VZf8gH7v3uo5SxjjIPPUA)
    ,
    [code](https://github.com/flexgp/gp-learners)
- Operon (Burlacu et al. 2020)
    [paper](https://dl.acm.org/doi/pdf/10.1145/3377929.3398099?casa_token=HJgFp342K0sAAAAA:3Xbelm-5YjcIgjMvqLcyoTYdB0wNR0S4bYcQBGUiwOuwqbFfV6YnE8YKGINija_V6wCi6dahvQ3Pxg)
    ,
    [code](https://github.com/heal-research/operon)

- Semantic Backpropagation GP (Virgolin et al. 2019)
    [paper](https://dl.acm.org/doi/pdf/10.1145/3321707.3321758?casa_token=v43VobsGalkAAAAA:Vj8S9mHAv-H4tLm_GCL4DJdfW3e5SVUtD6J3gIQh0vrNzM3s6psjl-bwO2NMnxLN0thRJ561OZ0sQA)
    ,
    [code](https://github.com/marcovirgolin/GP-GOMEA)

Methods Staged for Benchmarking:

- PySR (Cranmer 2020)
    [code](https://github.com/MilesCranmer/PySR)
- PSTree (Zhang 2021)
    [code](https://github.com/hengzhe-zhang/PS-Tree)
    

# References
- SRBench Repository : https://github.com/cavalab/srbench.git
- datasets : https://github.com/EpistasisLab/penn-ml-benchmarks)

A pre-print of the current version of the benchmark is available:
[v2.0](https://github.com/EpistasisLab/regression-benchmark/releases/tag/v2.0) was reported in our Neurips 2021 paper: 

La Cava, W., Orzechowski, P., Burlacu, B., de França, F. O., Virgolin, M., Jin, Y., Kommenda, M., & Moore, J. H. (2021). 
Contemporary Symbolic Regression Methods and their Relative Performance. 
_Neurips Track on Datasets and Benchmarks._
[arXiv](https://arxiv.org/abs/2107.14351),
[neurips.cc](https://datasets-benchmarks-proceedings.neurips.cc/paper/2021/hash/c0c7c76d30bd3dcaefc96f40275bdc0a-Abstract-round1.html)

[v1.0](https://github.com/EpistasisLab/regression-benchmark/releases/tag/v1.0) was reported in our GECCO 2018 paper: 

Orzechowski, P., La Cava, W., & Moore, J. H. (2018). 
Where are we now? A large benchmark study of recent symbolic regression methods. 
GECCO 2018. [DOI](https://doi.org/10.1145/3205455.3205539), [Preprint](https://www.researchgate.net/profile/Patryk_Orzechowski/publication/324769381_Where_are_we_now_A_large_benchmark_study_of_recent_symbolic_regression_methods/links/5ae779b70f7e9b837d392dc9/Where-are-we-now-A-large-benchmark-study-of-recent-symbolic-regression-methods.pdf)
