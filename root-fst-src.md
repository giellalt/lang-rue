
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
<small>This (part of) documentation was generated from [../src/fst/root.lexc](http://github.com/giellalt/lang-rue/blob/main/../src/fst/root.lexc)</small>