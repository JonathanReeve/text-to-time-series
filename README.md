# Text-to-time-series

Transforming a text into a collection of numerical time series for mathematical analysis. Work-in-progress. 

## Ideas for time series representations of text

 - Dialogue/narration (in quotation marks/not in quotation marks). 
   - TEI editions have this marked up. 
   - Could use [Stanford CoreNLP's QuoteAnnotator for identifying dialogue](https://stanfordnlp.github.io/CoreNLP/quote.html). 
 - Tree fragments 
   - see [this dissertation, containing a method for breaking a sentence into syntactic tree fragments](http://www.illc.uva.nl/Research/Publications/Dissertations/DS-2016-07.text.pdf) 
   - maybe of POS representations, Penn Treebank tags
   - For each word/lemma, count the number of child nodes in its sentence tree. Perhaps couple with the number of words in that sentence.
 - Ngrams 
   - also of POS, tags
 - Word embeddings
   - If embedding is into R^300, would take all 300 time series, one for each embedding coordinate, together
   - Could fix a vector (or collection of vectors) and take cosine similarity measurement from the fixed vector(s)

## Technical Notes

"Spatial" scales: 
 - Character (i.e., letter) 
 - Word / Lemma
 - Sentence
 - Paragraph
 - Chapter 
   - [Chapterize](https://github.com/JonathanReeve/chapterize) tool could be useful here
