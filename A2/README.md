Exercises and assignments for HCDE410: Human Data Interaction. Everything here is a work in progress unless otherwise noted :)
# A2: Exploring Sources of Bias in Data

## Overview
This assignment examines potential sources of bias in the Wikipedia
Talk Corpus. I analyze annotator demographics, check missing and
duplicate data, and discuss how these limitations could affect a
general-purpose toxic-speech detector.

I completed Questions 1–8 and the code option, Questions 9–12.

## Files
- `hcde410-a2.ipynb`: Code, results, and written answers.
- `toxicity_annotations.tsv`: Individual toxicity ratings and worker IDs.
- `wikipedia_datasets/toxicity_worker_demographics.tsv`:
  Toxicity worker demographics.
- `wikipedia_datasets/attack_worker_demographics.tsv`:
  Personal attack worker demographics.
- `wikipedia_datasets/aggression_worker_demographics.tsv`:
  Aggression worker demographics.
- `a2_all_annotator_demographics.csv`: Combined demographic records,
  exported by the notebook.

## Data Sources
The starter notebook and demographic files were provided through
HCDE 410 course materials. The toxicity annotation file was downloaded
from the original data release.

- [Toxicity dataset](https://figshare.com/articles/dataset/Wikipedia_Talk_Labels_Toxicity/4563973)
- [Personal attacks dataset](https://figshare.com/articles/dataset/Wikipedia_Talk_Labels_Personal_Attacks/4054689)
- [Aggression dataset](https://figshare.com/articles/dataset/Wikipedia_Talk_Labels_Aggression/4267550)
- [Dataset documentation](https://meta.wikimedia.org/wiki/Research:Detox/Data_Release)

## How to Run
Use Python 3 with Jupyter Notebook or JupyterLab and pandas.

Keep `toxicity_annotations.tsv` in the same directory as the notebook.
Keep the three demographic TSV files inside `wikipedia_datasets`
in that directory. If the annotation file is not included in the
repository, download it from the Toxicity dataset link above.

Open `hcde410-a2.ipynb` and run all cells from top to bottom.
The notebook generates `a2_all_annotator_demographics.csv`.

## Notes
The attack and aggression demographic files contain identical records,
so only one is included in the main demographic analysis. Worker IDs
are dataset-specific, so toxicity annotations are matched only with
toxicity worker demographics.

For Questions 10–11, I report both the share of annotation records
and the percentage of distinct comments covered by each group.
Comment coverage percentages can overlap because multiple workers
labelled each comment.

## AI Use
I used ChatGPT to troubleshoot the `random.sample()` compatibility
error and file-path errors, help write and explain analysis code,
find sources and identify relevant information for Q7, and help
draft and revise written responses.

## License and Acknowledgments
See `LICENSE.md` for applicable licensing information.
Original data and course materials retain their respective licenses
and terms. The starter notebook and assignment instructions were
provided by HCDE 410.