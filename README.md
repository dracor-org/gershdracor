# GerShDraCor
**Ger**man **Sh**akespeare **Dra**ma **Cor**pus. Edited by [Frank Fischer](https://lehkost.github.io/). This TEI-encoded corpus contains all 37 of Shakespeare's plays in their German translations, edited by Schlegel and Tieck, in the edition published by Aufbau-Verlag Berlin/Weimar (3rd edition 1975), which is based on the last edition published during Schlegel's lifetime (3rd edition 1843/44). The digitised print edition was obtained from [TextGrid Repository](https://hdl.handle.net/11858/00-1734-0000-0005-0B3F-D), which in turn is a TEI conversion of the [Zeno.org](http://www.zeno.org/nid/20005683920) digitisation. This collection provided an additional play (»Die beiden edlen Vettern«) that Shakespeare is now considered to have co-authored.

After a prolonged beta phase from 2021 to 2024, this corpus is now ready to join the other stable corpora in the DraCor ecosystem. Explore the corpus in the DraCor frontend: **https://dracor.org/gersh**

## To cite GerShDraCor …

… we suggest the following:

* Frank Fischer (ed.): German Shakespeare Drama Corpus (GerShDraCor): Shakespeare's plays in their German translations, edited by Friedrich Schlegel and Ludwig Tieck. Hosted on GitHub, 2021–. https://github.com/dracor-org/gershdracor

The corpus is released under the Creative Commons Zero copyright waiver ([CC0](https://creativecommons.org/public-domain/cc0/)).

We have made many adjustments and improvements, which we document in more detail below.

## Main benefits of this corpus
* Assignment of character IDs for all speaking instances, including groups and every secondary character (```particDesc```).
* Assignment of Wikidata IDs to characters, if applicable (mythological, historical, fictional characters).

The actual core of this digital edition is the introduction of character IDs, as is common in all DraCor corpora. This opens up possibilities for fine-grained digital analyses. It will be particularly useful for visualising and analysing the co-occurrence networks of the plays. Disambiguating all 1.497 characters was the most time-consuming part of the corpus work.

Although completed for the time being, the assignment of Wikidata IDs to characters can be regarded a work in progress as Wikidata improves. Please note that there are some composite characters in Shakespeare and that sometimes there are two entries per character in Wikidata (one for the theatrical character, one for the historical character on which it is based, cf. [Hamlet](http://www.wikidata.org/entity/Q2447542) vs. [Hamlet](http://www.wikidata.org/entity/Q462225)). Therefore, assigning a Wikidata ID is often contingent, our aim for now was to at least be consistent.

## Minor benefits
* Page breaks adjusted.
* Detailed bibliographic info added.
* Reintegrated text parts lost in the TextGrid conversion.
* Typos removed, especially regarding names.
* Introduced ```<role>``` and ```<roleDesc>``` in ```<castList>```.

It is important to emphasise that **this is not a critical edition**, but our attempt to optimise the existing digitised version of this corpus for computer-aided analysis using the tools of the digital humanities.

To this end, the TextGrid files have been streamlined. Bloated encoding has been removed to make the corpus more vanilla. We backported some text parts that were lost during the conversion from Zeno.org to TextGrid (example: the prologue to Act 2 in »Henry V.«, vol. 3, pp. 403–404, is missing in the [TextGrid conversion](http://www.textgridrep.org/textgrid:vnf1.0) compared to [Zeno.org](http://www.zeno.org/nid/20005689341)). We also corrected some typos compared to the print edition (without aiming for a complete revision). There are certainly still a few OCR errors hidden, especially in the italicised stage directions.

## Translators

In the Aufbau edition, names of (main) translators are given for each play, among those four:
* August Wilhelm Schlegel
* Ludwig Tieck
* Wolf Heinrich von Baudissin
* Dorothea Tieck

We have adopted this information, although the issue of translatorship in this case is extremely complex. The state of research on these translations is presented in this collected volume:

* Claudia Bamberg, Christa Jansohn, Stefan Knödler (eds.): Die Shakespeare-Übersetzungen August Wilhelm Schlegels und des Tieck-Kreises: Kontext – Geschichte – Edition. Berlin, Boston: De Gruyter 2023. ([doi:10.1515/9783111017419](https://doi.org/10.1515/9783111017419))

## Changelog
### 21.10.2021
* First beta version.
### 21.08.2024
* Assignment of character IDs completed. End of beta phase.
### 26.08.2024
* Assignment of Wikidata IDs to characters completed.
### 27.08.2024
* Enrich ```<castList>``` with ```<role>``` and ```<roleDesc>```.
