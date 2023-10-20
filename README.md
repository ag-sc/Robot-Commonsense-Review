# Commonsense Knowledge for Cognitive Robots: Supplementary Material

This repository contains supplementary material to the paper "Commonsense Knowledge for Cognitive Robots: A Systematic Literature Review", which is currently under review.

## Abstract

One of the big challenges in robotics is the generalisation necessary for performing unknown tasks in unknown environments on unknown objects.
For us humans, this challenge is simplified by the commonsense knowledge we can access. 
For cognitive robotics, representing and acquiring commonsense knowledge is a relevant problem, so we perform a systematic literature review to investigate the current state of commonsense knowledge application in cognitive robotics.
For this review, we combine a keyword search on six search engines with a snowballing search on six related reviews, resulting in 2048 distinct publications.
After applying pre-defined inclusion and exclusion criteria, we analyse the remaining 52 publications.
Our focus lies on the use cases and domains for which commonsense knowledge is employed, the commonsense aspects that are considered, the datasets / resources used as sources for commonsense knowledge and the methods for evaluating these approaches
Additionally, we discovered a divide in terminology between research from the knowledge representation and reasoning and the robotics community.
This divide is investigated by looking at the extensive review performed by Zech et al.[^1], with whom we have no overlapping publications despite the similar goals.

## Research Questions

Our paper aims at answering the following research questions by performing a systematic literature review following the principles and guidelines provided by Kitchenham and Charters[^2] and Okoli[^3]:
- **RQ1** For which use cases has the use of CSK been considered in robotics research?
- **RQ2** Which aspects of CSK have been considered? Which aspects of CSK have received less consideration?
- **RQ3** Which datasets or resources are mainly considered in robotics as a source for CSK?
- **RQ4** What methods are employed to assess the approaches? Which CSK datasets or resources are utilised in these evaluations?

## Search Methodology

An overview over our methodology can be seen in [this diagram](Images/SearchProcedure.pdf), which was created with the [PRISMA Shiny app](https://estech.shinyapps.io/prisma_flowdiagram/)[^4].
All necessary, additional information (e.g. in- and exclusion criteria) are collected in the [reviewprotocol](Reviewprotocol.pdf).

In general, we combine a keyword search using 4 keywords on 6 different search engines with a snowballing search on 6 related literature reviews.
From the resulting 2.048 publications, the duplicates are excluded and they are filtered regarding their metadata, leaving us with 1.472 different publications.
They are screened and filtered in two steps by first looking at their title and then at their abstract.
After both screening steps, 80 publications remain that were read completely.
Since one full version could not be accessed and 27 provided no relevant content for answering our research questions, we remain with 52 publications we analysed.

## Repository Structure
```bash
├── Data
│   ├── Duplicates.csv                # duplicate occurrences between the 36 different sources
│   ├── Final Publications.csv        # data for the 52 analysed publications
│   └── Publications Zech2019.csv     # 152 publications included in the review by Zech et al.
├── Images                            # folder containing all images created for the reviewprotocol and the paper
│   └── ...
├── References                        # .bib files containing the found publications (1x file per source)
│   ├── Keyword Search                # 24 results for the keyword search where each file combines a source with a keyword
│   │   └── ...                       
│   ├── Snowballing                   # 12 results for the snowballing search differentiated between ingoing and outgoing search
│   │   └── ...                       
│   └── Final Inclusion.bib           # bib file containing the 47 analysed publications
├── DataVisualization.ipynb           # jupyter notebook used for analysing the './Data' folder and creating the './Images'
├── Reviewprotocol.pdf                # the reviewprotocol documenting the systematic literature review
└── Screening & Analysis.ods          # spreadsheet documenting the in- and exclusion process through the different screening steps
```

## Disclaimer

This work is a collaboration between the [Semantic Computing Group](https://www.uni-bielefeld.de/fakultaeten/technische-fakultaet/arbeitsgruppen/semantic-computing/) at the Center for Cognitive Interaction Technology @ Bielefeld University, the [DICE group](https://dice-research.org/) @ Paderborn University and the [Institute for Artificial Intelligence](https://ai.uni-bremen.de/) @ University of Bremen. Please contact <a href="https://www.uni-bielefeld.de/fakultaeten/technische-fakultaet/arbeitsgruppen/semantic-computing/team/jan-philipp-toeberg/">Jan-Philipp Töberg</a> (jtoeberg(at)techfak(dot)uni-bielefeld(dot)de) for further information or collaboration.

## References

[^1]: P. Zech, E. Renaudo, S. Haller, X. Zhang, and J. Piater, ‘Action representations in robotics: A taxonomy and systematic classification’, The International Journal of Robotics Research, vol. 38, no. 5, pp. 518–562, Apr. 2019, doi: [10.1177/0278364919835020](https://doi.org/10.1177/0278364919835020).
[^2]: B. Kitchenham and S. Charters, ‘Guidelines for performing Systematic Literature Reviews in Software Engineering’, Keele University and University of Durham, 2007.
[^3]: C. Okoli, ‘A Guide to Conducting a Standalone Systematic Literature Review’, Communications of the Association for Information Systems, vol. 37, pp. 879–910, 2015, doi: [10.17705/1CAIS.03743](https://doi.org/10.17705/1CAIS.03743).
[^4]: N. R. Haddaway, M. J. Page, C. C. Pritchard, and L. A. McGuinness, ‘*PRISMA2020* : An R package and Shiny app for producing PRISMA 2020‐compliant flow diagrams, with interactivity for optimised digital transparency and Open Synthesis’, Campbell Systematic Reviews, vol. 18, no. 2, Jun. 2022, doi: [10.1002/cl2.1230](https://doi.org/10.1002/cl2.1230).
