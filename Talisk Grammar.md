# Talísk Grammar

Grammatically, [Talísk](https://github.com/Koennen/Conlangs/blob/main/Talisk.md)
is very regular. The
[Dime language's](https://en.wikipedia.org/wiki/Dime_language) practice of
marking case on noun phrases rather than nouns was the feature of the language
that struck me as the most interesting, and I implemented it here.

## General Prefixes

The negating prefix **na-** may attach to any type of word.

| Function               | Prefix     |
| ---------------------- | ---------- |
| \[plural]              | **ha-**    |
| \[negation]            | **na(h)-** |
| which?                 | **me-**    |
| \[proximal determiner] | **le-**    |
| \[distal determiner]   | **li-**    |

## Nouns

### Cases and Case Affixes

Affixes for case apply after any prefixes because they modify nouns as a whole.

| Case | Affix   |
| ---- | ------- |
| ABS  | \[null] |
| ERG  | **-il** |
| DAT  | **-ak** |
| GEN  | **ta-** |
| LOC  | **-em** |

## Verbs

### Forming Verbs

#### The Stem

All verbs in Talísk begin with a
[stem](https://github.com/Koennen/Conlangs/blob/main/Talisk%20Lexicon.md#verbs).
Verb stems are either intransitive (taking only one argument) or transitive
(taking two or more arguments). All transitive verbs in Talísk are strictly so,
and must take an agent, as the absence of one marks the
[antipassive](https://github.com/Koennen/Conlangs/blob/main/Talisk%20Grammar.md#the-antipassive).

#### Tense, Aspect, and Mood

Although I considered a tenseless language, Talísk has several tenses. These
suffixes can (with the exception of the
[aorist](https://en.wikipedia.org/wiki/Aorist)) be thought of as attaching onto
the present form.

| Tense      | Suffix   |
| ---------- | -------- |
| DIST. PAST | **-inu** |
| REC. PAST  | **-iku** |
| PRES       | **-i**   |
| AORIST     | **-e**   |
| PROX. FUT  | **-ike** |
| DIST. FUT  | **-ine** |

#### Verbal Suffixes

[Verbal suffixes](https://github.com/Koennen/Conlangs/blob/main/Talisk%20Lexicon.md#verbal-suffixes)
attach after the tense marker.

### The Reflexive

The reflexive pronoun **sil** may be used to describe a situation in which the
agent and patient of a transitive verb are the same.

**Sil naf ul-íku.**  
REFL\[ERG] 2\[ABS.SG] burn-REC.PST  
"You just burned yourself."  

#### Special Cases

##### The Reflexive and Intransitive Verbs

The reflexive pronoun may be used with intransitive verbs, especially those
describing a temporary state. Here the reflexive emphasizes the beginning or
end of that state. This usage is uncommon in formal speech.

**%Sil luk enk-í.**  
REFL\[ERG] 3\[ABS.SG] sit-PRS  
lit. "They seat themself."  
"They sit down."  

##### Alternate Interpretations

The reflexive pronoun *may* mark the omission of an agent in transitive clauses,
but this interpretation depends on the verb. Alternate interpretations (valid in
some dialects) are preceded with '%' to mark their rarity. (Most speakers would
use the
[indefinite](https://github.com/Koennen/Talisk/blob/main/Talisk%20Grammar.md#the-indefinite-simulating-the-passive)
to indicate these secondary meanings.)

**Sil talif ul-í.**  
REFL\[ERG] tree\[ABS.SG] burn-PRS  
lit. "A tree burns itself."  
%"A tree is burning."  

**Sil lusk lek-í.**  
REFL\[ERG] adult\[ABS.SG] see-PRS  
lit. "An adult sees themself."  
\%%"An adult is being seen."  

### The Antipassive

Like other ergative languages, Talísk has an
[antipassive](https://en.wikipedia.org/wiki/Antipassive_voice) voice, which
allows for the omission of the patient of a transitive verb by promoting the
agent to the absolutive case.

**Talif ul-í.**  
tree\[ABS.SG] burn-PRS  
"A tree burns \[it]."  

**Lusk lek-é.**  
adult\[ABS.SG] see-PRS  
"An adult sees \[things] (in general)."  

### The Indefinite: Simulating the Passive

Sometimes the agent of a transitive clause is unknown. In this case, the
indefinite **menil** may be used.

**Men-il talif ul-í.**  
thing-ERG tree\[ABS.SG] burn-PRS  
lit. "Something burns a tree."  
"A tree is burning."  

**Men-il lusk lek-í.**  
thing-ERG adult\[ABS.SG] see-PRS  
lit. "Something sees an adult."  
"An adult is being seen."  

## Syntax

Talísk is primarily SOV. Adjectives and numerals follow the nouns they modify,
and the last adjective in a noun phrase receives the case marking. Plurality is
not marked on noun phrases quantified by numerals.

Yes-no questions are SVO. Any declarative sentence may be transformed into a
question by using the interrogative prefix **me-** on a noun.

## Examples

**Le-dínd end-í.**  
PROX.DET-dog\[ABS.SG] sleep-PRS  
"This dog is sleeping."  

**Le-dínd ek end-é.**  
PROX.DET-dog\[ABS] two sleep-AOR  
"These two dogs sleep often."  

**Din-il talif ahun lek-íku.**  
1-ERG\[SG] tree\[ABS.SG] small see-REC.PST  
"I just saw a small tree."  

**Naf-il lek-í li-tálif ahun?**  
2-ERG\[SG] see-PRS DIST.DET-tree\[SG] small  
"Do you see that small tree?"  

* **Na-lek-í.**  
NEG-see-PRS  
"I do not see."  

**Luk-il lisk inin ud lut-ínu.**  
3-ERG\[SG] person large three\[ABS] hear-DIST.PST  
"They (sg.) heard three large persons."  

**Li-dínd ek-il ha-náf in-íne.**  
DIST.DET-dog two-ERG PL-2\[ABS] kill-DIST.FUT  
"Those two dogs will eventually kill you all."  

**Naf-il lek-í dind?**  
2-ERG\[SG] see-PRS dog\[ABS.SG]  
"Do you see a dog?"  

**Ha-dín-il talk at klef-í.**  
PL-2-ERG stone one\[ABS] throw-PRS  
"We throw one stone (implies that everyone's hands were on that one stone,
helping to throw it)."  

**Ha-dín-il talk at klef-í-si.**  
PL-2-ERG stone one\[ABS] throw-PRS-DISTR  
"We each throw one stone (at the same time)."  

**Naf-il me-dínd lek-í?**  
2-ERG\[SG] WH.DET-dog\[ABS.SG] see-PRS  
"Which dog do you see?"  

**Li-lísk-il talif ihak dus-íku naf-ak.**  
DIST.DET-person-ERG\[SG] tree four\[ABS] give-REC.PST 2-DAT\[SG]  
"That person just gave you four trees."  

**Dind ta-dín-il na-half-íne.**  
{dog\[SG] GEN-1\[SG]}-ERG NEG-fly-DIST.FUT  
"My dog will never fly."  

**Lusk ihak del-ínu dind ahun-ak.**  
adult four\[ABS] laugh-DIST.PST dog\[SG] small-DAT  
"Four adults laughed at a small dog."  

**Li-ha-mínk nak-é sles-em.**  
DIST.DET-PL-child\[ABS] swim-AOR water-LOC\[SG]  
"Those children often swim in the water."  

**Sil sulk uhed kenal-é ha-féts nehuln-em.**  
REFL\[ERG] adolescent five\[ABS] bind-AOR PL-cliff black-LOC  
"Five teenagers have sex (lit. 'bind themselves') (at no particular instant) at
some black cliffs."  
