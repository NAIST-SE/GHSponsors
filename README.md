# Research Artifact: An Exploratory Study of GitHub Sponsors Early Adoption
This is a research artifact for the ICSE'22 paper "GitHub Sponsors: Exploring a New Way to Contribute to Open Source". The following three research questions were constructed to guide the study.

* RQ1: *Who participates in GitHub Sponsors?*
    * RQ1.1: *What are the characteristics of sponsored developers?*
    * RQ1.2: *What are the characteristics of sponsors?*
* RQ2: *What characteristics make developers more likely to receive sponsorship?*
* RQ3: *What are developers' perceived challenges and benefits related to sponsoring?*
    * RQ3.1: *Why are develpers looking for sponsors?*
    * RQ3.2: *What is the impact of (not) getting sponsorship?*
    * RQ3.3: *Why are developers sponsoring?*

This artifact is a repository including a list of studied repositories on GitHub, a dataset for the network diagram for answering RQ1, the features for sponsored and non-sponsored developers for RQ2, the features for sponsors for RQ2, and survey material and response for RQ3.

<br>

## Contents
* `repositories` - datasets of studied repositories
    * `10_or_more.csv` - 1,168,856 repositories that have 10 stars or more
    * `9_or_less.csv` - 1,338,533 repositories that have 9 stars or less

* `survey` - survey materials
    * `not_sponsored.pdf` - survey for non-sponsored developers
    * `sponsored.pdf` - survey for spnsored developers
    * `sponsoring.pdf` - survey for sponsors

* `README.md` - this file

* `metrics.csv` - features for sponsored and non-sponsored developers

* `network.csv` - dataset for network diagram

* `sponsoring.csv` - features for sponsors

<br>

## Details
### metrics.csv
The CSV file about statuses of sponsored and non-sponsored developers.
* `is_sponsored` - Mark 1 if the developer has resistered to GitHub Sponsors
* `lang` - The language of developer
* `num_repos` - The number of repositories developer commited
* `num_own_repos` - The number of repositories developer own
* `num_repos_top_contributing` - The number of repositories that developer is ranked as top in terms of commits
* `highest_stars` - The highest number of stars in the repositories that developer contributed to
* `num_sponsoring` - The number of accounts that developer is sponsoring
* `num_repos_top_co_contributing` - The number of repositories that developer contributed to with the top number of commits, and that have at least one sponsor in the same repository

### network.csv
The CSV file be used for network graph in RQ1.
* `sponsor` - The developer who is sponsoring
* `to` - The developer who is sponsored
* `spo_language` - The language of the developer who is sponsoring
* `to_language` - The language of the developer who is sponsored

### sponsoring.csv
The CSV file about statuses of sponsoring developers.
* `num_repos` - The number of repositories developer commited
* `num_own_repos` - The number of repositories developer own
* `top_star` - The highest number of stars in the repositories that developer contributed to
* `num_sponsoring` - The number of accounts that developer is sponsoring

### survey/non-sponsored.csv
The CSV file about responses of non-sponsored survey.

### survey/sponsored.csv
The CSV file about responses of sponsored survey.

### survey/sponsoring.csv
The CSV file about responses of sponsoring survey.
