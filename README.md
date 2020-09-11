# Lessing Sentiment And Emotion Corpus

This repository contains the corpus that was developed as part of an annotation study further described in the paper <a href="https://epub.uni-regensburg.de/37486/1/annDH18_after_Review_%2BExpertAnnotations_mb_v3.pdf">Sentiment Annotation of Historic German Plays: An Empirical Study on Annotation Behavior"</a> by 
<ul>
  <li><a href="https://www.uni-regensburg.de/sprache-literatur-kultur/medieninformatik/sekretariat-team/thomas-schmidt/index.html">Thomas Schmidt</a></li>
  <li><a href="https://ch.uni-leipzig.de/burghardt/">Manuel Burghardt</a></li>
  <li><a href="https://www.germanistik.uni-wuerzburg.de/ndl1/mitarbeiter/dennerlein/">Katrin Dennerlein</a></li> 
</ul>
The paper and corpus was presented at the <a href="http://ceur-ws.org/Vol-2155/">Workshop on Annotation in Digital Humanities (annDH 2018)</a> in Sofia, Bulgaria. The annoted text is German.

## Citation Information

If you use or reference this corpus in any shape or form please cite the paper:

Schmidt, T., Burghardt, M. & Dennerlein, K. (2018). Sentiment Annotation of Historic German Plays: An Empirical Study on Annotation Behavior. In: Sandra Kübler, Heike Zinsmeister (eds.), <em>Proceedings of the Workshop on Annotation in Digital Humanities (annDH 2018)</em> (pp. 47-52). Sofia, Bulgaria. <a href="https://epub.uni-regensburg.de/37486/1/annDH18_after_Review_%2BExpertAnnotations_mb_v3.pdf">[pdf]</a> <a href="https://epub.uni-regensburg.de/cgi/export/eprint/37486/BibTeX/epub-eprint-37486.bib">[bibtex]</a> 

## Corpus Description

This corpus was created via a sentiment and emotion annotation study. You can find more information about the annotation procedure, the used scheme and agreement and distribution results in the paper. The speeches are originally from plays that were gathered via the platform <a href="https://textgrid.de/">Textgrid</a>.

The corpus consists of 200 semi-randomly selected speeches of all of Lessing's plays that were annotated independently by 5 annotators. The csv-file consists of 200 lines, one for each speech, the annotations of all five annotators and the majority decision among them.

We used the following schemes to annotate the speeches:
- binary polarity (negative/positive)
- differentiated polarity (very negative/negative/positive/very positive/neutral/mixed)
- present/not_present for 8 basic emotions (Anger, Anticipation, Disgust, Fear, Joy, Sadness, Surprise, Trust)

### Columns

The most important columns of the csv-file are the <br>Rated_Speech</br>, which is the text that was rated and the <br>Majorityannotation_Polarity_binary</br> and <br>Majorityannotation_Polarity_differentiated</br> which are the majority annotations for these schemes. The following list summarizes all columns of the table.

- <b>ID</b>: an id for every speech
- <b>Title_of_Play</b>: the name of the play the speech is from; every play is represented in regards to the overall size of the play compared to the entire corpus meaning shorter plays are represented with less plays, longer with more
- <b>Position_in_play</b>: Act-, scene- and speech-number of the speech
- <b>Predecessor_Speech</b>: the speech before the speech to be rated (name of speaker included)
- <b>Rated_Speech</b>: the speech that was rated concerning sentiment information (name of speaker included)
- <b>Successor_Speech</b>: the speech after the speech that was rated (name of speaker included)
- <b>Majorityannotation_Polarity_binary</b>: negative/positive; what at least three of the five annotators selected for the binary sentiment annotation meaning rather positive or negative; this is the annotation we finally used for our sentiment analysis evaluation
- <b>Annotation1_Polarity_binary</b>: negative/positive; the binary polarity annotation by annotator 1
- <b>Annotation2_Polarity_binary</b>: negative/positive; the binary polarity annotation by annotator 2
- <b>Annotation3_Polarity_binary</b>: negative/positive; the binary polarity annotation by annotator 3
- <b>Annotation4_Polarity_binary</b>: negative/positive; the binary polarity annotation by annotator 4
- <b>Annotation5_Polarity_binary</b>: negative/positive; the binary polarity annotation by annotator 5
- <b>Majorityannotation_Polarity_differentiated</b>: very negative/negative/positive/very positive/mixed/neutral/no_majority; if at least three of the five annotators have the same annotation a polarity attribution is assigned otherwise no_majority is assigned
- <b>Annotation1_Polarity_differentiated</b>: negative/positive; the differentiated polarity annotation by annotator 1
- <b>Annotation2_Polarity_differentiated</b>: negative/positive; the differentiated polarity annotation by annotator 2
- <b>Annotation3_Polarity_differentiated</b>: negative/positive; the differentiated polarity annotation by annotator 3
- <b>Annotation4_Polarity_differentiated</b>: negative/positive; the differentiated polarity annotation by annotator 4
- <b>Annotation5_Polarity_differentiated</b>: negative/positive; the differentiated polarity annotation by annotator 5
- <b>Annotation{1-5}_{Anger, Anticipation, Disgust, Fear, Joy, Sadness, Surprise, Trust}</b>: present/not_present; if the specific emotion is present or not present in the rated speech

## Further Reading
Besides the above paper you can find out more about this corpus and analysis we performed with it in the following papers:

Schmidt, T. & Burghardt, M. (2018). An Evaluation of Lexicon-based Sentiment Analysis Techniques for the Plays of Gotthold Ephraim Lessing. In: <em>Proceedings of the Second Joint SIGHUM Workshop on Computational Linguistics for Cultural Heritage, Social Sciences, Humanities and Literature</em> (pp. 139-149). Santa Fe, New Mexico: Association for Computational Linguistics. <a href="https://www.aclweb.org/anthology/W18-4516.pdf">[pdf]</a>

Schmidt, T. & Burghardt, M. (2018). Toward a Tool for Sentiment Analysis for German Historic Plays. In: Piotrowski, M. (ed.), <em>COMHUM 2018: Book of Abstracts for the Workshop on Computational Methods in the Humanities 2018</em> (pp. 46-48). Lausanne, Switzerland: Laboratoire laussannois d'informatique et statistique textuelle. <a href="https://epub.uni-regensburg.de/37575/1/ComHum2018-Epub-Version.pdf">[pdf]</a>

Schmidt, T., Burghardt, M. & Dennerlein, K. (2018). „Kann man denn auch nicht lachend sehr ernsthaft sein?“ – Zum Einsatz von Sentiment Analyse-Verfahren für die quantitative Untersuchung von Lessings Dramen. In <em>Book of Abstracts, DHd 2018</em>. <a href="https://epub.uni-regensburg.de/37579/1/Self-Archiving-Version_DHd-2018.pdf">[pdf]</a>

