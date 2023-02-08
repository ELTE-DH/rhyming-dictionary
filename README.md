# Rhyming Dictionary of Hungarian Canonical poetry:

The rhyming dictionary were generated automatically on the basis of [_ELTE Poetry Corpus_](https://github.com/ELTE-DH/poetry-corpus), which is a database containing all the poems of 50 Hungarian canonical writers with the annotations of grammatical properties and poetic features related to sound devices.

## Formats:

- rhyming\_dictionary\_XML.zip: The compressed file contains the XML version of the rhyming dictionary. The file must be unzipped after downloading.
- rhyming_dictionary.tsv: The TSV file contains the rhyming dictionary in a tabular format. This version is suitable for use in spreadsheet software.
- rhymingDict_PDF: The folder contains the PDF version of the rhyming dictionary in several files. This version is suitable for manual reading.

## Elements and attributes of the XML:

- `<entry>`: each entry in the rhyming dictionary contains all the rhyme pairs occurring with a given lemma, together with the information below
- `<entryLemma>`: lemma
- `<rhymePairs>`: containing all of the rhyme pairs with the lemma in `<entryLemma>`
- `<rhymePair>`: containing a specific rhyme pair
   - `@between_rhymes`: number of lines rhyming with the rhyming pair between the two words of the rhyming pair
   - `@distance`: distance of the two rhyming words
   - `@poem_id`: ID of the poem in which the rhyme pair occurs 
   - `@stanza_id`: ID of the stanza in which the rhyme pair occurs 
- `<rhymeWord1>`: one rhyming word in the rhyme pair
   - `@lemma`: lemma
   - `@msd`: morphosyntactic features ([Universal Dependencies](https://universaldependencies.org/))
   - `@numSyll`: syllable number
   - `@phonStruct`: phonological representation of the word
        - `c`: consonant
        - `b`: short back vowel
        - `B`: long back vowel
        - `f`: short front vowel
        - `F`: long front vowel
   - `@phonType`: type of vowels in the word
        - `low`: only back vowels in the word
        - `high`: only front vowels in the word
        - `mixed`: front and back vowels in the word
   - `@pos`: part of speech ([Universal Dependencies](https://universaldependencies.org/))
   - `@word_id`: ID of the word in ELTE Poetry Corpus
- `<rhymeWord2>`: the other rhyming word in the rhyme pair
- `<author>`: author of the poem in which the rhyme pair occurs
- `<title>`: title of the poem in which the rhyme pair occurs 
- `<url>`: URL of the poem in which the rhyme pair occurs

## The columns of the TSV:

- `wordform1`: one rhyming word in the rhyme pair
- `wordform2`: the other rhyming word in the rhyme pair
- `lemma1`: lemma of wordform1
- `pos1`: part of speech of wordform1
- `lemma2`: lemma of wordform2
- `pos2`: part of speech of wordform2
- `between_rhymes`: number of lines rhyming with the rhyming pair between the two words of the rhyming pair
- `distance`: distance of the two rhyming words 
- `author`: author of the poem in which the rhyme pair occurs
- `title`: title of the poem in which the rhyme pair occurs 
- `stanza_id`: ID of the stanza in which the rhyme pair occurs 
- `poem_id`: ID of the poem in which the rhyme pair occurs 
- `url`: URL of the poem in which the rhyme pair occurs

## The fields of the PDF files:

__rhyming\_word\_1 – rhyming\_word\_2__ (lemma1, part\_of\_speech\_1 – lemma2, part\_of_speech\_2), Author: _The first 4 words of the poem title_ serial number of the stanza (distance of the two rhyming words, number of lines rhyming with the rhyming pair between the two words of the rhyming pair)

## Creator:

[Péter Horváth](https://github.com/horvathpeti99)

## License:

The content of the repository is licensed under the [CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license.



