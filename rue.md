


















* Sets for POS sub-categories





* Sets for Semantic tags





* Sets for Morphosyntactic properties






































































































































































* Sets for verbs


- V is all readings with a V tag in them, REAL-V should
be the ones without an N tag following the V.  
The REAL-V set thus awaits a fix to the preprocess V ... N bug.



* The set COPULAS is for predicative constructions







* NP sets defined according to their morphosyntactic features







* The PRE-NP-HEAD family of sets

These sets model noun phrases (NPs). The idea is to first define whatever can
occur in front of the head of the NP, and thereafter negate that with the
expression **WORD - premodifiers**.












The set **NOT-NPMOD** is used to find barriers between NPs.
Typical usage: ... (*1 N BARRIER NPT-NPMOD) ...
meaning: Scan to the first noun, ignoring anything that can be
part of the noun phrase of that noun (i.e., "scan to the next NP head")






* Miscellaneous sets





















* Border sets and their complements













* Syntactic sets




These were the set types.



## HABITIVE MAPPING


* **hab1** 


* **hab2** 

* **hab3** (<hab> @ADVL>) for hab-actor and hab-case; if leat to the right, and Nom to the right of leat. Lots of restrictions.



* **habNomLeft** 


* **hab4** 	



* **hab6** 

* **hab7** 

* **hab8** This is not HAB
* **hab5**  This is not HAB



* **habDain** (<hab> @ADVL>) for (Pron Dem Pl Loc) if leat followed by Nom to the right




* **habGen** (<hab> @<ADVL) hab for Gen; if Gen is located in the end of the sentence and Nom is sentence initial










































































* **spred<obj** (@SPRED<OBJ) for Acc; the object of an SPRPED. Not to be mistaken with OPRED. If SPRED is to the left, and copulas is to the left of it. Nom or Hab are found sentence initially.


* **Hab<spred** (@<SPRED) for Nom; if copulas, goallut or jápmit is FMAINV and habitive or human Loc is found to the left. OR: if Ill or @Pron< followed by HAB are found to the left.

* **Hab>Advlcase<spred** (<ext> @<SUBJ) for Nom; it allows adverbials with Ill/Loc/Com/Ess to be found inbetween HAB and <ext>.

* **Nom>Advlcase<spred** (<ext> @<SUBJ) for Nom; it allows adverbials with Ill/Loc/Com/Ess to be found inbetween Nom and <ext> @<SUBJ.

* **<spred** (<ext> @<SUBJ) for Nom; if copulas to the left, and some kind of adverb, N Loc, time related word or Po to the left of it. OR: if Ill or @Pron< to the left, followed by copulas and the before mentioned to the left of copulas. 

* **<spred** (<ext> @<SUBJ) for Nom, but not for Pers. To the left boahtit or heaŋgát as MAINV, and futher to the left is some kind of place related word, or time related word


* **<spredQst1** (<ext> @<SUBJ) for Nom in a typically question sentence; if A) Hab, some kind of place word, Po or Nom to the left, and Qst followed by copulas to the left. B) same as a, only the Qst-pcle is attached to copulas. C) Qst to the left, with copulas to its left, but not if two Nom:s are found somewhere to the right. D) copulas to the left, and BOS to the left. E) Loc or Ill to the left, and Loc or Hab to the left of this, Qst and copulas to the left. F) Num @>N to the left, Hab, some kind of place word, Po or Nom to the left, and Qst followed by copulas to the left. NOTE) for all these rules; human, Loc or Sem/Plc not allowed to the right.

* **<spredQst2** (@<SPRED) for Nom; in a typically question sentence; differs from <spredQst1 by not beeing as restricted to the right. Though you are not allowed to be Pers or human.

* **Nom<spredQst** (@<SPRED) for Nom; in a typically question sentence. Differs from <spredQst2 by letting Nom be found between SPRED and copulas



* **<spred** (@<SPRED) for A Nom or N Nom if; the subject Nom is on the same side of copulas as you: on the right side of copulas

* **<spredVeara** (@<SPRED) for veara + Nom; if genitive immediately to the right, and intransitive mainverb to the right of genitive

* **leftCop<spred** (@<SPRED) for Nom; if copulas is the main verb to the left, and there is no Ess found to the left of cop (note that Loc is allowed between target and cop). OR: if you are Coll or Sem/Group with copulas to your left. 

* **<spredLocEXPERIMENT** (@<SPRED) for material Loc; if you are to the right of copulas, and the Nom to the left of copulas is not a hab-actor


* **NumTime** (@<SPRED) for A Nom

* **<spredSg** (@<SPRED) for Sg Nom	

* **<spredPg** (@<SPRED) for Pl Nom	

* **<spred** (@<SPRED) for Nom; if copulas to the left, and Nom or sentence boundary to the left of copulas. First one to the right is EOS.

* **<spred** (@<SPRED) for N Ess

* **spredEss>** (@SPRED>) for N Ess; if copulas to the right of you, and if an NP with nom-case first one to your left.

* **HABSpredSg>** (@SPRED>) for Nom; if habitive first one to the left, followed by copulas.

* **GalleSpred>** (@SPRED>) for Num Nom; if sentence initial

* **spredSgMII>** (@SPRED>)

* **r492>** (@SPRED>) for Interr Gen; consisting only of negations. You are not allowed to be MII. You are not allowed to have an adjective or noun to yor right. You are not allowed to have a verb to your right; the exception beeing an aux.



* **AdjSpredSg>** (@SPRED>) for A Sg Nom; if copulas to the right, but not if A or @<SPRED are found to the right of copulas

* **SpredSg>Hab** (@SPRED>) for Nom; if you are sentence initial, copulas is located to the right, and there is a habitive to the right of copulas



* **Spred>SubjInf** (@SPRED>) for Nom; if copulas to the right, and the subject of copulas is an Inf to the right

* **spredCoord** (@<SPRED) coordination for Nom; only if there already is a SPRED to the left of CNP. Not if there is some kind of comparison involved.






* **subj>Sgnr1** (@SUBJ>) for Nom Sg, including Indef Nom if; VFIN + Sg3 or Pl3 to the right (VFIN not allowed to the left) 

* **subj>Du** (@SUBJ>) for dual nominatives, including Coll Nom. VFIN + Du3 to the right. 
* **subj>Pl** (@SUBJ>) for plural nominatives, including Coll and Sem/Group. VFIN + Pl3 to the right.

* **subj>Pl** (@SUBJ>) for plural nominatives


* **subj>Sgnr2** (@SUBJ>) for Nom Sg; if VFIN + Sg3 to the right.

* **<subjSg** (@<SUBJ) for Nom Sg; if VFIN Sg3 or Du2 to the left (no HAB allowed to the left).




















* **f<advl** (@-F<ADVL) for infinite adverbials

* **f<advl** (@-F<ADVL) for infinite adverbials



* **s-boundary=advl>** (@ADVL>) for ADVL that resemble s-booundaries. Mainverb to the right.




* **-fobj>** (@-FOBJ>) for Acc 

* **-fobj>** (@-FOBJ>) for Acc




* **advl>mainV** (@ADVL>) if; finite mainverb not found to the left, but the finite mainverb is found to the right.


* **<advl** (@<ADVL) if; finite mainverb found to the left. Not if a comma is found immediately to the left and a finite mainverb is located somewhere to the right of this comma.




* **<advlPoPr** (@<ADVL) if mainverb to the left.
* **advlPoPr>** (@<ADVL) if mainverb to the right.



* **advlEss>** (@<ADVL) for weather and time Ess, if FMAINV to the left.






* **advl>inbetween** (@ADVL>) for Adv; if inbetween two sentenceboundaries where no mainverb is present.

* **comma<advlEOS** (@<ADVL) if; comma found to the left and the finite mainverb to the left of comma. To the right is the end of the sentence.



* **advlBOS>** (@ADVL>) if; you are N Ill and found sentnece initially. First one to your right is a clause.


* **<advlPoEOS** (@<ADVL) for Po; if you are found at the very end of a sentence. A mainverb is needed to the right though.



* **cleanupILL<advl** (@<ADVL) for N Ill if; there are no boundarysymbols to your left, if you arent already @N< OR @APP-N<, and no mainverb is to yor left.











* **<opredAAcc** (@<OPRED) for A Acc; if an other accusative to the left, and a transtive verb to the left of it. OR: if a transitive verb to the left, and an accusative to the left of it.


### sma object









* **<advlEss** (@<ADVL) for ESS-ADVL if; FMAINV to the left
* **<spredEss** (@<SPRED) for N Ess if; FMAINV to the left is intransitive or bargat





## SUBJ MAPPING - leftovers

## OBJ MAPPING - leftovers


## HNOUN MAPPING















* * *
<small>This (part of) documentation was generated from [../src/cg3/functions.cg3](http://github.com/giellalt/lang-rue/blob/main/../src/cg3/functions.cg3)</small>Noun inflection
The Rusyn language nouns inflect in cases.

* * *
<small>This (part of) documentation was generated from [../src/fst/affixes/nouns.lexc](http://github.com/giellalt/lang-rue/blob/main/../src/fst/affixes/nouns.lexc)</small>
INTRODUCTION TO MORPHOLOGICAL ANALYSER OF Rusyn LANGUAGE.


 # Definitions for Multichar_Symbols

## Symbols that need to be escaped on the lower side (towards twolc): (copied from sme)



## Markers

 * ¹ ² ³ ⁴ ⁵ ⁶ ⁷ ⁸ ⁹ ⁰  = Used to enumerate homonymous lemmas
 * %>    = End-of-stem marker (nominals)
 * %<    = End-of-stem marker (verbs)

## POS
 * +A       = Adjective
 * +Abbr    = Abbreviation
 * +Adv     = Adverb
 * +CC      = Coordinating conjunction
 * +CS      = Subordinating conjunction
 * +Det     = Determiner
 * +Interj  = Interjection
 * +N       = Noun
 * +Num     = Numeral
 * +Paren   = Parenthetical вводное слово
 * +Pcle    = Particle
 * +Po      = Postposition (ради is the only postposition)
 * +Pr      = Preposition
 * +Pron    = Pronoun
 * +V       = Verb

## Sub-POS
 * +All     = All: весь
 * +Coll    = Collective numerals
 * +Def     = Definite
 * +Dem     = Demonstrative
 * +Indef   = Indefinite: кто-то, кто-нибудь, кто-либо, кое-кто, etc.
 * +Interr  = Interrogative: кто, что, какой, ли, etc.
 * +Neg     = Negative: никто, некого, etc.
 * +Pers    = Personal
 * +Pos     = Possessive, e.g. его, наш
 * +Prcnt   = Percent
 * +Prop    = Proper
 * +Recip   = Reciprocal: друг друга
 * +Refl    = Pronoun себя, possessive свой
 * +Rel     = Relativizer, e.g. который, где, как, куда, сколько, etc.
 * +Symbol = independent symbols in the text stream, like £, €, ©

## Verbal MSP
 * +Impf +Perf        = Imperfective, perfective
 * +IV +TV            = Intransitive, transitive (Zaliznjak does not mark trans-only, so transitive verbs all have both TV and IV)
 * +Inf +Imp          = Imperatives: 2nd person = читай, 1st person = прочитаем
 * +Pst +Prs +Fut     = Past, present, future
 * +Sg1 +Sg2 +Sg3     = person sg
 * +Pl1 +Pl2 +Pl3     = person pl
 * +PrsAct +PrsPss    = Participles (+PrsAct+Adv and +PstAct+Adv are used for the verbal adverbs)
 * +PstAct +PstPss    = Participles
 * +Pass              = Passive
 * +Imprs             = Impersonal (cannot have explicit subject)
 * +Lxc             = Lexicalized (for participial forms)

 * +Der             = Derived (for participial forms)
 * +Der/PrsAct             = Derived (for participial forms)
 * +Der/PrsPss             = Derived (for participial forms)
 * +Der/PstAct             = Derived (for participial forms)
 * +Der/PstPss             = Derived (for participial forms)

## Nominal MSP
 * +Msc +Fem +Neu +MFN   = grammatical gender,  +MFN = gender unspecifiable (pl tantum)
 * +Inan +Anim +AnIn     = animacy (+AnIn = ambivalent animacy for non-accusative modifiers)
 * +Sem/Sur +Sem/Pat     = Surname (фамилия), Patronymic
 * +Sem/Ant +Sem/Alt     = Anthroponym/Given name, Other
 * +Sg +Pl               = number
 * +Nom +Acc +Gen       
 * +Loc +Dat +Ins       
 * +Loc2 +Gen2 +Voc     
 * +Count                = Count (for человек/людей or лет/годов, etc. also шага́/шара́/часа́/etc.)
 * +Ord      = Ordinal
 * +Cmpar    = Comparative
 * +Sint     = Synthetic comparative is possible, e.g. старее
 * +Pred     = "Predicate", also used for short-form adjectives
 * +Cmpnd    = "Compound", used for compounding adjectives, such as русско-английский
 * +Att      = Attenuative comparatives like получше, поновее, etc.

## Punctuation
 * +PUNCT    = Punctuation
 * +CLB    = Clause boundary  ! TODO SENT vs CLB which is which?
 * +SENT    = Clause boundary
 * +COMMA   = Comma
 * +DASH    = Dash
 * +LQUOT    = Left quotation
 * +RQUOT    = Right quotation
 * +QUOT    = "Ambidextrous" quotation
 * +LPAR     = Left parenthesis/bracket
 * +RPAR     = Right parenthesis/bracket
 * +LEFT     = Left parenthesis/bracket/quote/etc.
 * +RIGHT     = Right parenthesis/bracket/quote/etc.

## Other tags
 * +Prb      = +Prb(lematic): затруднительно - предположительно - нет
 * +Fac      = Facultative
 * +PObj     = Object of preposition (prothetic н: него нее них)
 * +Epenth   = epenthesis on prepositions (о~об~обо or в~во)
 * +Leng     = Lengthened доброй~доброю (marks less-canonical wordform that has more syllables)
 * +Elid     = Elided (Иванович~Иваныч, новее~новей, чтобы~чтоб, или~иль, коли~коль)
 * +Use/NG   = Do not generate (used for apertium, etc.)
 * +Use/Obs  = Obsolete
 * +Use/Ant  = Antiquated "устаревшее"
 * +Err/Orth  = Spelling (orthographic) error


* * *
<small>This (part of) documentation was generated from [../src/fst/root.lexc](http://github.com/giellalt/lang-rue/blob/main/../src/fst/root.lexc)</small>Nouns
Nouns in the Rusyn language are things.


*morning examples:*
* *рано:* `рано+N+Sg+Nom`
* *рана:* `рано+N+Pl+Nom`

* * *
<small>This (part of) documentation was generated from [../src/fst/stems/nouns.lexc](http://github.com/giellalt/lang-rue/blob/main/../src/fst/stems/nouns.lexc)</small>















































% komma% :,      Root ;
% tjuohkkis% :%. Root ;
% kolon% :%:     Root ;
% sárggis% :%-   Root ; 
% násti% :%*     Root ; 

* * *
<small>This (part of) documentation was generated from [../src/transcriptions/transcriptor-numbers-digit2text.lexc](http://github.com/giellalt/lang-rue/blob/main/../src/transcriptions/transcriptor-numbers-digit2text.lexc)</small>


We describe here how abbreviations are in Rusyn are read out, e.g.
for text-to-speech systems.

For example:

 * s.:syntynyt # ;  
 * os.:omaa% sukua # ;  
 * v.:vuosi # ;  
 * v.:vuonna # ;  
 * esim.:esimerkki # ; 
 * esim.:esimerkiksi # ; 


* * *
<small>This (part of) documentation was generated from [../src/transcriptions/transcriptor-abbrevs2text.lexc](http://github.com/giellalt/lang-rue/blob/main/../src/transcriptions/transcriptor-abbrevs2text.lexc)</small>