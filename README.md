# Text-to-time-series

Transforming a text into a collection of numerical time series for mathematical analysis. 

## Ideas for time series representations of text

 - Dialogue/narration (in quotation marks/not in quotation marks). TEI editions have this marked up. Could use [Stanford CoreNLP's QuoteAnnotator for identifying dialogue](https://stanfordnlp.github.io/CoreNLP/quote.html). 
 - Tree fragments 
   - see [this dissertation, containing a method for breaking a sentence into syntactic tree fragments](http://www.illc.uva.nl/Research/Publications/Dissertations/DS-2016-07.text.pdf)) 
   - maybe of POS representations, Penn Treebank tags
 - Ngrams 
   - also of POS, tags

## Technical Notes

"Spatial" scales: 
 - Character (i.e., letter) 
 - Word / Lemma
 - Sentence
 - Paragraph
 - Chapter ([chapterize](https://github.com/JonathanReeve/chapterize) tool could be useful here)
