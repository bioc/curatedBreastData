# curatedBreastData 2.42.0

## SIGNIFICANT USER-VISIBLE CHANGES

- The datasets are no longer stored in the package. They are hosted on
  Zenodo (https://zenodo.org/records/21415886), downloaded on first use,
  and cached with `BiocFileCache` (#1, @lwaldron).
- The package is no longer marked deprecated, and the startup deprecation
  warning is removed.

## NEW FEATURES

- New functions `getCuratedBreastDataExprSetList()` and `getClinicalData()`
  retrieve the Zenodo datasets (#1, @lwaldron).
- A small test dataset in `inst/extdata` allows offline examples and tests
  (#2, @lwaldron).
- `curatedBreastData_pData`, the pre-concatenated phenotype table, is now
  documented in the reference index and vignette.
- New pkgdown site.

## BUG FIXES AND MINOR IMPROVEMENTS

- Fix operator-precedence bugs in loops, and use `seq_along()`,
  `seq_len()` and `vapply()` (in `collapseDupProbes()`).
- Fix cache path handling in `BiocFileCache` retrieval when the cache is
  empty.
- Documentation is migrated to roxygen2, the vignette is converted to R
  Markdown, `DESCRIPTION` gains `biocViews`, `URL` and `BugReports`, and CI
  is added (#1, @lwaldron).

# curatedBreastData 0.99.0

- Initial package release.
