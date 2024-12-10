# Bank Failure Investigation

> An application of classical natural language processing and knowledge graphs.

## Motivation

I met with a banker the other day and found myself thinking about all kinds of data that there must be about banks. For no other reason than mere curiosity, I stumbled upon FDIC's list of failed banks and began to wonder why banks fail in the first place? I found myself browsing FDIC's Office of Inspector General's website for some intel. As of December 2024, 98 material loss reviews were published on the website.

I'm lazy, so I'm not about to download and read each report manually. So, I've decided to let Python do the heavy lifting instead.

Data mining to the rescue!

## Project Description

I downloaded 98 reports from the FDIC OIG website and read them using Python. I first tried to analyze the summary generated by using spaCy and creating a knowledge graph but later decided to do all of the text in ints entirety and just stick with ngrams extraction.

![Knowledge Graph](https://github.com/ecdedios/bank-failures/blob/main/viz/knowledge_graph.png)

## Findings

The most interesting insight is the frequent mention of "cre adc loan" in the corpora, which suggests a relationship of CRE and ADC loans to why banks are failing.

![CRE ADC Loan](https://github.com/ecdedios/bank-failures/blob/main/viz/trigram.png)

## Data

https://www.fdicoig.gov/reports-publications/bank-failures

## Reference

https://www.tandfonline.com/doi/full/10.1080/23322039.2023.2251272

## Usage

Written in Python 3.12. Libraries/packages and technologies used:

- notebook
- selenium
- beautiful soup
- pandas
- pypdf2 / pymupdf
- nltk
- spacy
- gensim
- scikit-learn

To see the project in action, open and run the notebooks or peruse the visuals in the viz directory.

## Meta

Ednalyn C. De Dios – [@ecdedios](https://github.com/ecdedios)

Distributed under the MIT license. See `LICENSE` for more information.

- LinkedIn: [in/ecdedios/](https://www.linkedin.com/in/ecdedios/)
- Resumé: [http://ednalyn.com](http://ednalyn.com)
- Data Science Projects [https://datasciencenerd.us](https://datasciencenerd.us)

## Contributing

1. Fork it (<https://github.com/ecdedios/bank-failures/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request

2024
