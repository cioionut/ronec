# RONEC - the Romanian Named Entity Corpus 

Version 1.0 of this free corpus holds **5127** sentences, annotated with **16** classes, with a total of **26376** annotated entities. The corpus comes into two formats: BRAT and CONLLUP, stored in the `roner/` folder. The CONLLUP file is annotated with lemma, POSes and dependency parsing information with [NLP-Cube](https://github.com/adobe/NLP-Cube). For more deatils regarding the corpus please see its dedicated [corpus info file](ronec/README.md).

### CONLLUP version: [What is CONLLUP?](http://universaldependencies.org/ext-format.html)
**Direct download of the text file(~14MB): [ronec.conllup](ronec/conllup/ronec.conllup)**

Example of an annotated sentence (annotations are in the last column, in the PARSEME:MWE annotation format):

``Peste 200000 de pelerini au asistat, la Lourdes, la liturghia în aer liber oficiată de Suveranul Pontif cu ocazia praznicului Adormirii Maicii Domnului.``

<pre>
1	Peste	peste	ADP	Spsa	AdpType=Prep|Case=Acc	2	advmod	_	_	*
2	200000	200000	NUM	Mc-p-d	Number=Plur|NumForm=Digit|NumType=Card	4	nummod	_	_	1:NUMERIC_VALUE
3	de	de	ADP	Spsa	AdpType=Prep|Case=Acc	2	case	_	_	*
4	pelerini	pelerin	NOUN	Ncmp-n	Definite=Ind|Gender=Masc|Number=Plur	6	nsubj	_	_	2:PERSON
5	au	avea	AUX	Va--3p	Number=Plur|Person=3	6	aux	_	_	*
6	asistat	asista	VERB	Vmp--sm	Gender=Masc|Number=Sing|VerbForm=Part	0	root	_	SpaceAfter=No	*
7	,	,	PUNCT	COMMA	_	9	punct	_	_	*
8	la	la	ADP	Spsa	AdpType=Prep|Case=Acc	9	case	_	_	*
9	Lourdes	Lourdes	PROPN	Np	_	6	obl	_	SpaceAfter=No	3:GPE
10	,	,	PUNCT	COMMA	_	9	punct	_	_	*
11	la	la	ADP	Spsa	AdpType=Prep|Case=Acc	12	case	_	_	*
12	liturghia	liturghie	NOUN	Ncfsry	Case=Acc,Nom|Definite=Def|Gender=Fem|Number=Sing	6	obl	_	_	*
13	în	în	ADP	Spsa	AdpType=Prep|Case=Acc	14	case	_	_	*
14	aer	aer	NOUN	Ncms-n	Definite=Ind|Gender=Masc|Number=Sing	12	nmod	_	_	*
15	liber	liber	ADJ	Afpms-n	Definite=Ind|Degree=Pos|Gender=Masc|Number=Sing	14	amod	_	_	*
16	oficiată	oficia	VERB	Vmp--sf	Gender=Fem|Number=Sing|VerbForm=Part	12	acl	_	_	*
17	de	de	ADP	Spsa	AdpType=Prep|Case=Acc	18	case	_	_	*
18	Suveranul	suveran	NOUN	Ncmsry	Case=Acc,Nom|Definite=Def|Gender=Masc|Number=Sing	16	nmod:agent	_	_	4:PERSON
19	Pontif	pontif	ADJ	Np	_	18	nmod	_	_	4
20	cu	cu	ADP	Spsa	AdpType=Prep|Case=Acc	21	case	_	_	*
21	ocazia	ocazie	NOUN	Ncfsry	Case=Acc,Nom|Definite=Def|Gender=Fem|Number=Sing	16	obl	_	_	*
22	praznicului	praznic	NOUN	Ncmsoy	Case=Dat,Gen|Definite=Def|Gender=Masc|Number=Sing	21	nmod	_	_	*
23	Adormirii	adormire	NOUN	Ncfsoy	Case=Dat,Gen|Definite=Def|Gender=Fem|Number=Sing	22	nmod	_	_	5:EVENT
24	Maicii	maică	NOUN	Ncfsoy	Case=Dat,Gen|Definite=Def|Gender=Fem|Number=Sing	23	nmod	_	_	5
25	Domnului	domn	NOUN	Ncmsoy	Case=Dat,Gen|Definite=Def|Gender=Masc|Number=Sing	23	nmod	_	SpaceAfter=No	5
26	.	.	PUNCT	PERIOD	_	6	punct	_	SpaceAfter=No	*
</pre>

### BRAT version: [What is BRAT?](http://brat.nlplab.org/)
The BRAT format comes ready-to-use in the BRAT annotator. The corpus is pre-split into 20 sub-folders. Just clone this repo and copy the `ronec/brat/` contents into the BRAT annotator's `data/` folder.

## Helper scripts

We also release a set of Python3 scripts in the `scripts/` folder. The `main.py` file contains one-liner functions that read, write and convert to/from BRAT/CONLLUP formats. More info regarding the scrips is found in [its Jupyter notebook](scripts/examples.ipynb).

## Authors
+ [Stefan Daniel Dumitrescu](https://www.linkedin.com/in/stefandumitrescu/)
+ [Andrei Avram](https://ro.linkedin.com/in/andrei-marius-avram-80698a169) 
+ [Luciana Morogan](https://www.linkedin.com/in/luciana-morogan-a7879568/)
+ [Stefan Toma](https://www.linkedin.com/in/stefan-adrian-toma-00a6b770/)

## Credits
A paper will be published in the following months. 

