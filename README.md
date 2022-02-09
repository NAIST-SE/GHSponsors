# Research Artifact - GitHub Sponsors: Exploring a New Way to Contribute to Open Source
[![DOI](https://zenodo.org/badge/447130568.svg)](https://zenodo.org/badge/latestdoi/447130568)

This is a research artifact for the ICSE'22 paper "**GitHub Sponsors: Exploring a New Way to Contribute to Open Source**". The following three research questions were constructed to guide the study.

* RQ1: *Who participates in GitHub Sponsors?*
    * RQ1.1: *What are the characteristics of sponsored developers?*
    * RQ1.2: *What are the characteristics of sponsors?*
* RQ2: *What characteristics make developers more likely to receive sponsorship?*
* RQ3: *What are developers' perceived challenges and benefits related to sponsoring?*
    * RQ3.1: *Why are develpers looking for sponsors?*
    * RQ3.2: *What is the impact of (not) getting sponsorship?*
    * RQ3.3: *Why are developers sponsoring?*

This artifact is a repository including lists of studied repositories on GitHub, a dataset for the network diagram for answering RQ1, the features for sponsored and non-sponsored developers for RQ2, the features for sponsors for RQ2, and survey material and coding of responses for RQ3.

## Contents
- `repositories` - lists of studied repositories
    * `10_or_more.csv` - 1,168,856 repositories with 10 stars or more
    * `9_or_less.csv` - 1,338,533 repositories with 9 stars or less
- `survey` - survey materials and results
    * `not_sponsored.pdf` - [survey form for non-sponsored developers](https://forms.gle/uHbjXzBv2WWwvaaW7)
    * `sponsored.pdf` - [survey form for spnsored developers](https://forms.gle/TkXwnyNc6vtxcwLX6)
    * `sponsoring.pdf` - [survey form for sponsors](https://forms.gle/4kkyTv7KaF3HCoRaA)
    * `not_sponsored.csv` - survey result of non-sponsored developers
    * `sponsored.csv` - survey result of spnsored developers
    * `sponsoring.csv` - survey result of sponsors
- `LICENSE.md` - [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/)
- `README.md` - this file
- `STATUS.md` - application of artifact badges of reusable and available
- `metrics.csv` - features of sponsored and non-sponsored developers
- `network.csv` - data for network diagram
- `paper.pdf` - the accepted paper
- `sponsoring.csv` - features of sponsors

## Details
### metrics.csv
Features of sponsored and non-sponsored developers.
* `is_sponsored` - 1 if the developer had been sponsored
* `lang` - Developer's main language
* `num_repos` - Number of repositories committed by the developer
* `num_own_repos` - Number of repositories owned by the developer
* `num_repos_top_contributing` - Number of repositories where the developer ranks among the top in terms of commits
* `highest_stars` - Number of stars for the repository with the highest number of stars contributed by the developer
* `num_sponsoring` - Number of developers sponsored by the developer
* `num_repos_top_co_contributing` - Number of repositories where the developer ranks among the top in terms of commits, and that have at least one sponsor in the same repository

### network.csv
Metrics used in the network graph.
* `sponsor` - The developer who was sponsoring
* `to` - The developer who was sponsored by the sponsor
* `spo_language` - The main language of the developer who was sponsoring
* `to_language` - The main language of the developer who was sponsored

### sponsoring.csv
Features of sponsors.
* `num_repos` - Number of repositories committed by the sponsor
* `num_own_repos` - Number of repositories owned by the sponsor
* `top_star` - Number of stars for the repository with the highest number of stars contributed by the sponsor
* `num_sponsoring` - Number of developers sponsored by the sponsor

## Coding schema for the survey
### Why are you looking for sponsors?
* `funding a particular feature/ product` - We used this code if the respondent mentioned something in particular (other than the OSS project itself) that they were planning to use the donations for, e.g., ''Fund hosting costs for hosted projects.''   
* `gauge interest/satisfaction` - Some respondents indicated using sponsorship as a way to receive feedback from the community, in particular to assess the community's interest in the project, e.g., ''To measure the degree of satisfaction with my OSS works.'' 
* `motivation` - We used this code if respondents were aware that receiving motivations would increase their motivation, e.g., ''It highly motivates me if I get money as donations for my work.''
* `recognition/ appreciation` - If respondents expressed that they wanted to give the community a way to express appreciation or recognition, we used this code, e.g., ''Why not, mostly. Mostly boils down to recognition for the work since the monetary amounts are negligible.''  
* `financial support in general terms` - In cases where respondents gave a somewhat generic answer related to making money, we used this code, e.g., ''to fund my open source work.''
* `none` - For respondents who did not mention a reason in response to the question, we used the code 'none'.

### Are you doing anything special to attract sponsors?
* `perks for sponsors` - For responses which mentioned a specific perk that was only available to sponsors of their work, we used this code, e.g., ''I offer short consulting sessions (just a 30-60 minute video call) for higher tier sponsors.''
* `social media` - We used this code if respondents mentioned a specific social media site or social media in general, e.g., ''Twitter - tweet about my work.''
* `written content on GitHub` - Responses which mentioned updating documentation to make their work more attractive to sponsors, we used this code, e.g., ''I've written out my goals more publicly.''
* `none` - If respondents did not mention any activities, we coded the response as 'none'.


### How has having sponsors affected you and the projects you are working on?/ How does the lack of sponsoring affect you and the projects you are working on?
* `better project quality` - We used this code for responses which mentioned a positive impact of sponsoring towards specific quality attributes, e.g., ''It’s made me feel a lot more motivated towards adding more open source code, and paying a higher level of attention to detail.''
* `limited effort` - This code was used for responses which mentioned a negative impact of the lack of sponsorship on the effort they were willing or able to spend, e.g., ''the projects receive less attention due to the need to do paid work.''
* `motivation` - Responses mentioning the impact of (lack of) sponsorship on motivation received this code, e.g., ''Some pressure to finish the project.''
* `satisfaction` - We used a similar category for responses related to satisfaction, e.g., ''Just for my heart's pleasure.''
* `need other channels` - Responses which indicated that a lack of sponsorship via GitHub Sponsors implied that they used other sponsorship platforms fall into this category, e.g., ''I have people making contribution via other channels.''
* `need other income` - Similarly, responses mentioning the need to look for other income in the absence of GitHub sponsorship were given its own code, e.g., ''I have to work on closed source and less interesting projects.''
* `other` - For any answer to the question that did not fit the above categories, we used the code 'other'.
* `none` - If the question was not answered, we coded it as 'none'.

### Why are you sponsoring others?/ Why did you become a sponsor?
* `dependencies/ benefited otherwise` - We used this code for responses which explicitly mentioned dependencies or other benefits, e.g., ''My project uses their projects.''
* `excellent work` - If respondents indicated that they sponsored because of excellent projects, we used this code, e.g., ''I want to contribute to great projects.''
* `form of involvement` - Related to the previous point, if respondents indicated that they see sponsoring as a form of involvement, we used this code, e.g., ''I had no more time to help with coding, so I decided to sponsor.''
* `fairness/ give back to community` - We used this code if the main reason was related to fairness rather towards the community, e.g., ''If someone provides OSS software which I daily use, I think it's fair and important to pay a contribution.''
* `set example` - Going a step further, some respondents mentioned that they sponsor to set an example for others, e.g., ''I want to set an example for other developers that large numbers of even small supporters can make an impact on keeping the OS community sustainable.''
* `sustain project/ community` - If the response focused on using sponsorship to sustain a project or the community as a while, we used this code, e.g., ''To help them sustain their OSS software.''
* `recognition/ appreciation` - If the responses mentioned recognizing a project or member of the community, or to show appreciation, we used this code, e.g., ''To praise their work, and recognize their invested time.''
* `motivation` - Some respondents explicitly mentioned targeting the motivation of developers with their donations, e.g., ''Because I understand how hard it is to stay motivated.''
* `required to get access to features/ training` - If participants mentioned sponsoring in return for specific access, we used this code, e.g., ''It was required to access training videos.''
* `generic help/ support` - Somewhat generic statements such as ''Help valuable users in community'' received this code.
* `other` - If the response did not fit any of these categories, we coded it as 'other'.

### What are the effects of your sponsorship? Are the effects as you expected?
* `collective` - We used this code for responses which explicitly mentioned that their contributions on their own would not make a difference while the collective might, e.g., ''I do not expect to affect anyone with 1 USD a month. The collective does, but I personally don't have a say necessarily, which is good.''
* `fund particular activities` - If respondents expected particular activities to take place in return for their sponsoring, we used this code, e.g., ''Maybe better handling of my files Issues. Also to keep a project alive.''
* `grateful/ motivated developers` - Responses related to the motivation of the developers receiving sponsorship received this code, e.g., ''I'm not actually sure how to measure it. I just hope that provides enough signal to them to feel motivated.''
* `recognition as sponsor` - We used this code for responses mentioning recognition of sponsors, e.g., ''Yes, as part of some sponsorships, we get our org some badges in their repo, to showcase our support.''
* `required to get access to features/ training` - If the intended effect of sponsorship was to get access to certain features, we used this code, e.g., ''Getting involved in email threads and invitations to beta testing.''
* `satisfaction` - Responses from sponsors mentioning their own satisfaction received this code, e.g., ''I honestly don’t get much out of sponsoring except personal satisfaction.''
* `sustain project` - If the main effect was sustaining a particular project, we used this code, e.g., ''That keep the product alive and maintained.'' 
* `none` - If respondents did not mention any effect, we coded it as 'none'.

## Authors
* [Naomichi Shimada](https://github.com/naomichi-s)
* [Tao Xiao](https://tao-xiao.github.io/)
* [Hideaki Hata](https://hideakihata.github.io/)
* [Christoph Treude](http://ctreude.ca/)
* Kenichi Matsumoto
