# Traditional-OLAP-Paper
Welcome new PR, please conform to the committed rules:  paperName(with link) [MeetingName Year]

If the paper has the open-source code, please supply its github links in Meeting.

- [Traditional-OLAP-Paper](#traditional-olap-paper)
  - [Query-Aware Database Generation](#query-aware-database-generation)
  - [Query Optimization](#query-optimization)
    - [Cardinality Estimation](#cardinality-estimation)
    - [Join Order](#join-order)
    - [Join Algorithms](#join-algorithms)
    - [Cost Model](#cost-model)
    - [View](#view)
    - [Survey](#survey)
    - [Index](#index)
  - [Query Exection](#query-exection)
  - [Query Compilation](#query-compilation)
  - [Logic Bugs Detection](#logic-bugs-detection)

## Query-Aware Database Generation
1.  [QAGen: Generating Query-Aware Test Databases](https://cs.uwaterloo.ca/~tozsu/publications/other/sigmod07-final.pdf) [SIGMOD 2007]
2.  [Generating Targeted Queries for Database Testing](https://dl.acm.org/doi/pdf/10.1145/1376616.1376668) [SIGMOD 2008]
3. [Generating Databases for Query Workloads](https://dl.acm.org/doi/pdf/10.14778/1920841.1920950) [VLDB 2010]
4. [Data Generation using Declarative Constraints](https://dl.acm.org/doi/pdf/10.1145/1989323.1989395) [SIGMOD 2011]
5. [MyBenchmark: generating databases for query workloads](https://link.springer.com/article/10.1007/s00778-014-0354-1) [VLDB Journal 2014]
7. [Scalable and Dynamic Regeneration of Big Data Volumes](https://openproceedings.org/2018/conf/edbt/paper-114.pdf) [EDBT 2018]
8. [Touchstone: Generating Enormous Query-Aware Test Databases](https://www.usenix.org/system/files/conference/atc18/atc18-li-yuming.pdf) [OSDI 2018]
9. [Projection-Compliant Database Generation](https://www.vldb.org/pvldb/vol15/p998-sanghi.pdf) [VLDB 2022]
10. [SAM: Database Generation from Query Workloads with Supervised Autoregressive Models](https://dl.acm.org/doi/pdf/10.1145/3514221.3526168) [[SIGMOD 2022](https://github.com/Jamesyang2333/SAM)]

## Query Optimization
1. [Kepler: Robust Learning for Parametric Query Optimization](TODO) [SIGMOD 2023]
### Cardinality Estimation
1. [Access path selection in a relational database management system](https://courses.cs.duke.edu/compsci516/cps216/spring03/papers/selinger-etal-1979.pdf) [SIGMOD 1979]
2. [Equi-Depth Histograms For Estimating Selectivity Factors For Multi-Dimensional Queries](https://dl.acm.org/doi/pdf/10.1145/971701.50205) [None 1987]
3. [Optimal Histograms for Limiting Worst-Case Error Propagation in the Size of Join Results](https://dl.acm.org/doi/pdf/10.1145/169725.169708) [ACM Transactions on Database Systems 1993]
4. [Approximating multi-dimensional aggregate range queries over real attributes](https://dl.acm.org/doi/pdf/10.1145/335191.335448) [SIGMOD 2000]
5. [Independence is good: Dependency-based histogram synopses for high-dimensional data]() [SIGMOD 2001]
6. [The history of histograms (abridged)](https://www.vldb.org/conf/2003/papers/S02P01.pdf) [VLDB 2003]
7. [Selectivity estimators for multidimensional range queries over real attributes](https://cs.gmu.edu/~carlotta/publications/vldb090.pdf) [VLDB 2005]
8. [Join Over Histograms](http://www.adellera.it/static_html/investigations/join_over_histograms/JoinOverHistograms.pdf) [Alberto Dell'Era 2007]
9. [LHist: Towards Learning Multidimensional Histogram for Massive Spatial Data](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9458896) [ICDE 2021]
10. [A multi-dimensional histogram for selectivity estimation and fast approximate query answering](https://dl.acm.org/doi/pdf/10.5555/961322.961374) [CASCON 2003]
11. [STHoles: a multidimensional workload-aware histogram](http://www.cs.columbia.edu/~gravano/Papers/2001/sigmod01b.pdf) [SIGMOD 2001]
12. [Consistent histogram construction using query feedback](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=55708905fb9ecd1ffa2f41638410f672147ccdaa) [ICDE 2006]
13. [Improving accuracy and robustness of self-tuning histograms by subspace clustering](https://dbis.ipd.kit.edu/download/MineClusSTHoles_-_Minor_Revision.pdf) [ICDE 2016]
14. [Two-Level Sampling for Join Size Estimation](https://15721.courses.cs.cmu.edu/spring2023/papers/18-costmodels/p759-chen.pdf) [SIGMOD 2017]
15. [JoinSketch: A Sketch Algorithm for Accurate and Unbiased Inner-Product Estimation](TODO) [SIGMOD 2023]
16. [Efficient and Effective Cardinality Estimation for Skyline Family](TODO) [SIGMOD 2023]


### Join Order
1. [Efficiently Computing Join Orders with Heuristic Search](TODO) [SIGMOD 2023]
2. [Detecting Logic Bugs of Join Optimizations in DBMS](TODO) [SIGMOD 2023]
3. [Ready to Leap (by Co-Design)? Join Order Optimisation on Quantum Hardware](TODO) [SIGMOD 2023]

### Join Algorithms
1. [Massively Parallel Sort-Merge Joins in Main Memory Multi-Core Database Systems](https://15721.courses.cs.cmu.edu/spring2023/papers/12-sortmergejoins/p1064-albutiu.pdf) [VLDB 2012]
2. [Free Join: Unifying Worst-Cast Optimal and Traditional Joins](https://arxiv.org/pdf/2301.10841.pdf) [arXiv 2023]


### Cost Model
1. [LEO – DB2’s LEarning Optimizer](https://15721.courses.cs.cmu.edu/spring2023/papers/18-costmodels/stillger-vldb2001.pdf) [VLDB 2011]
2. [Predicting query execution time: are optimizer cost models really unusable?](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6544899) [ICDE 2013]
3. [Forecasting the cost of processing multi-join queries via hashing for main-memory databases](https://arxiv.org/pdf/1507.03049.pdf) [SoCC 2015]
4. [Query Performance Prediction for Concurrent Queries using Graph Embedding](http://www.vldb.org/pvldb/vol13/p1416-zhou.pdf) [VLDB 2020]
5. [Efficient Deep Learning Pipelines for Accurate Cost Estimations Over Large Scale Query Workload](https://arxiv.org/pdf/2103.12465.pdf) [arXiv 2021]


### View
1. [Foreign Keys Open the Door for Faster Incremental View Maintenance](TODO) [SIGMOD 2023]

### Survey
1. [Cardinality Estimation: An Experimental Survey](https://www.vldb.org/pvldb/vol11/p499-harmouch.pdf) [VLDB 2017]
2. [A Survey on Advancing the DBMS Query Optimizer: Cardinality Estimation, Cost Model, and Plan Enumeration](https://arxiv.org/pdf/2101.01507.pdf) [VLDB 2021]
3. [Have query optimizers hit the wall?](https://link.springer.com/article/10.1007/s00778-021-00689-y) [VLDB Journal 2022]
4. [Cardinality Estimation in DBMS: A Comprehensive Benchmark Evaluation](https://dl.acm.org/doi/pdf/10.14778/3503585.3503586) [VLDB 2022]
5. [Data dependencies for query optimization: a survey](https://link.springer.com/article/10.1007/s00778-021-00676-3) [VLDB Journal 2022]


### Index
1. [SQL Server Column Store Indexes](https://15721.courses.cs.cmu.edu/spring2023/papers/04-olapindexes/p1177-larson.pdf) [SIGMOD 2011]
2. [Column Sketches: A Scan Accelerator for Rapid and Robust Predicate Evaluation](https://15721.courses.cs.cmu.edu/spring2023/papers/04-olapindexes/hentschel-sigmod18.pdf) [SIGMOD 2018]

## Query Exection
1. [Materialization Strategies in the Vertica Analytic Database: Lessons Learned](https://15721.courses.cs.cmu.edu/spring2023/papers/06-execution/shrinivas-icde2013.pdf) [ICDE 2013] 
2. [Access Path Selection in Main-Memory Optimized Data Systems: Should I Scan or Should I Probe?](https://15721.courses.cs.cmu.edu/spring2023/papers/06-execution/kester-sigmod17.pdf) [SIGMOD 2017]

## Query Compilation
1. [How to Architect a Query Compiler](https://15721.courses.cs.cmu.edu/spring2023/papers/09-compilation/shaikhha-sigmod2016.pdf) [SIGMOD 2016]
2. [Adaptive Execution of Compiled Queries](https://15721.courses.cs.cmu.edu/spring2023/papers/09-compilation/kohn-icde2018.pdf) [ICDE 2018]

## Logic Bugs Detection

1. [Detecting Logic Bugs of Join Optimizations in DBMS ]()[SIGMOD 2023 Best Paper]
