
# Version 1.2.0 (2019-7-30)

* Downsampling of count matrices using binomial thinning implemented in `estimateParam()` (UMI-read ratio estimation) and `simulateDE()`.
* Setup of DE simulations now in one function (`Setup()`) instead of two.
* `estimateParam()` with additional filtering options based on quality control checkup of scater package.
* implement sctransform as a single cell normalisation method.

# Version 1.1.3 (2018-07-10)

* `simulateDE()` using SCnorm scaling factors as weights in limma-trend, limma-voom.

# Version 1.1.2 (2018-06-20)

* `estimateParam()` error fixed concerning expression cleanup.
* precompiled vignette in inst/doc/.

# Version 1.1.1 (2018-04-19)

* `simulateDE()` now with the option to perform DE testing on filtered/imputed counts (option `DEFilter`)

# Version 1.1.0 (2018-03-29)

* simulation of batch effects (see options `p.B`, `bLFC` and `bPattern` in `DESetup()` and `simulateCounts()`)
* simulation of spike-in expression (see `estimateSpike` , `plotSpike` and option `spikeIns` in `simulateDE` and `simulateCounts()`)
* simulation of multiple sample groups (e.g. single cell populations) with `simulateCounts()`
* imputation and prefiltering options prior to normalisation in DE power simulations added (scImpute, scone, Seurat, DrImpute, SAVER)
* additional normalisation options and DE tools (esp. for single cells) included in `simulateDE()`
* evaluation of simulation setup using estimated versus true value comparisons of library size factors and log2 fold changes in `evaluateSim()` and `plotEvalSim()`
* increased flexibility in preprocessing for distribution evaluation in `evaluateDist()`

