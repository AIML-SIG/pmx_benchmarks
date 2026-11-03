# Benchmark Submission

## Submission Track

Which goal does this submission target? (check one)

- [ ] **Goal 1 — Generic Benchmark** (teaching case, agentic dataset, unit-test style, moderate novelty)
- [ ] **Goal 2 — Grand Challenge** (highly realistic drug-development problem, proposed scientific review)

Not sure? See [Scope & Eligibility](https://aiml-sig.github.io/pmx_benchmarks/scope.html).

---

## Benchmark Information

**Dataset Name:**
**Authors:**
**Brief Description:**

---

## Motivation *(required for all submissions)*

> Why should this dataset be added to this repository?

<!-- Your answer here -->

> Which existing datasets (in this repo or elsewhere) are most similar?

<!-- Your answer here -->

> How is this submission concretely different enough to warrant inclusion?

<!-- Your answer here -->

---

## Submission Checklist

### Required Files

- [ ] `benchmarks/<dataset-name>/index.qmd` with all required sections (including Motivation)
- [ ] `benchmarks/<dataset-name>/data/train.csv`
- [ ] `benchmarks/<dataset-name>/data/test.csv`
- [ ] `benchmarks/<dataset-name>/data/data-dictionary.yml` (yspec-style YAML)
- [ ] `benchmarks/<dataset-name>/metadata.yml` with `goal` field set

### Documentation

- [ ] Abstract clearly describes the benchmark
- [ ] Motivation section is present (see above)
- [ ] Background and context are provided
- [ ] Data generation process is documented (for synthetic data)
- [ ] All variables described with units in the data dictionary
- [ ] Tasks clearly defined with metrics and output formats
- [ ] Train/test split rationale is explained
- [ ] References included where appropriate

### Data Quality

- [ ] Train and test files use consistent column structure
- [ ] Data dictionary covers all columns
- [ ] No personally identifiable information (PII) included
- [ ] For Goal 2, data is longitudinal or an exception is justified
- [ ] For Goal 2, sampling, relationships, and dropout or missingness reflect the problem where relevant

### Task Requirements

- [ ] At least one task defined with `type`, `output_format`, and `metric`
- [ ] Evaluation performed on the test set
- [ ] Tasks fit the selected track: focused questions for Goal 1, motivated drug-development decisions for Goal 2

### Metadata

- [ ] All required fields completed
- [ ] `goal` field set (`generic` or `grand_challenge`)
- [ ] YAML syntax is valid
- [ ] Authors and affiliations are accurate
- [ ] `license: MIT` set (the repository default — discuss eligibility before submission if you cannot use MIT)

### Technical

- [ ] Quarto builds successfully: `quarto render benchmarks/<dataset-name>/index.qmd`
- [ ] Validation scripts pass: `python .github/scripts/validate_benchmark.py`
- [ ] All links in documentation work
- [ ] File naming follows conventions (lowercase-with-dashes)

---

## Additional Information

### Related Publications or Preprints

<!-- List any related publications or preprints -->

### Notes for Reviewers

<!-- Optional: context, known limitations, or open questions -->

---

## For Maintainers

- [ ] Automated validation passed
- [ ] Review appropriate to the selected track completed
- [ ] Documentation quality approved
- [ ] Citation information recorded; DOI requested if the archival process is available
- [ ] Benchmark listing updated on website
