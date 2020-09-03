# Lessing Sentiment And Emotion Corpus

This repository contains the corpus that was developed as part of an annotation study further described in the paper <a href=https://epub.uni-regensburg.de/37486/1/annDH18_after_Review_%2BExpertAnnotations_mb_v3.pdf>"Sentiment Annotation of Historic German Plays: An Empirical Study on Annotation Behavior"</a> by <a href="https://www.uni-regensburg.de/sprache-literatur-kultur/medieninformatik/sekretariat-team/thomas-schmidt/index.html">Thomas Schmidt</a>, <a href="">Manuel Burghardt</a> and <a href="">Katrin Dennerlein</a>. The paper and corpus was presented at the <a href="">Workshop on Annotation in Digital Humanities (annDH 2018)</a> in Sofia, Bulgaria. The annoted text is German.

## Citation Information

If you use or reference this corpus in any shape or form please cite the paper:

Schmidt, T., Burghardt, M. & Dennerlein, K. (2018). Sentiment Annotation of Historic German Plays: An Empirical Study on Annotation Behavior. In: Sandra Kübler, Heike Zinsmeister (eds.), Proceedings of the Workshop on Annotation in Digital Humanities (annDH 2018) (pp. 47-52). Sofia, Bulgaria.

<ul>
  <li><a href="">Link to the paper</a></li>
  <li><a href="">Link to the presentation at the workshop</a></li>
<ul>

## Corpus Description

This corpus was created via a sentiment and emotion annotation study. You can find more information about the annotation procedure, the used scheme and agreement and distribution results in the paper. The speeches are originally from plays that were gathered via the platform Textgrid.

The corpus consists of 200 semi-randomly selected speeches of all of Lessing's plays that were annotated independently by 5 annotators. The csv-file consists of 200 lines, one for each speech.

We used the following schemes to annotate the speeches:
- binary polarity (negative/positive)
- differentiated polarity (very negative/negative/positive/very positive/neutral/mixed)

### Columns
- ID: an id for every speech
- Title_of_Play: the name of the play the speech is from; every play is represented in regards to the overall size of the play compared to the entire corpus meaning shorter plays are represented with less plays, longer with more
- Position_in_play: Act-, scene- and speech-number of the speech
- Predecessor_Speech: the speech before the speech to be rated (name of speaker included)
- Rated_Speech: the speech that was rated concerning sentiment information (name of speaker included)
- Successor_Speech: the speech after the speech that was rated (name of speaker included)
- Majorityannotation_Polarity_binary: negative/positive; what at least three of the five annotators selected for the binary sentiment annotation meaning rather positive or negative; this is the annotation we finally used for our sentiment analysis evaluation
- Annotation1_Polarity_binary: negative/positive; the binary polarity annotation by annotator 1
- Annotation2_Polarity_binary: negative/positive; the binary polarity annotation by annotator 2
- Annotation3_Polarity_binary: negative/positive; the binary polarity annotation by annotator 3
- Annotation4_Polarity_binary: negative/positive; the binary polarity annotation by annotator 4
- Annotation5_Polarity_binary: negative/positive; the binary polarity annotation by annotator 5
- Majorityannotation_Polarity_differentiated: very negative/negative/positive/very positive/mixed/neutral/no_majority; if at least three of the five annotators have the same annotation a polarity attribution is assigned otherwise no_majority is assigned
- Annotation1_Polarity_differentiated: negative/positive; the differentiated polarity annotation by annotator 1
- Annotation2_Polarity_differentiated: negative/positive; the differentiated polarity annotation by annotator 2
- Annotation3_Polarity_differentiated: negative/positive; the differentiated polarity annotation by annotator 3
- Annotation4_Polarity_differentiated: negative/positive; the differentiated polarity annotation by annotator 4
- Annotation5_Polarity_differentiated: negative/positive; the differentiated polarity annotation by annotator 5
