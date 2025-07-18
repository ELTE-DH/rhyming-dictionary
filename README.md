# Rhyming Dictionary of Hungarian Canonical poetry:

The rhyming dictionary were generated automatically on the basis of [_ELTE Poetry Corpus_](https://github.com/ELTE-DH/poetry-corpus), which is a database containing all the poems of 53 Hungarian canonical writers with the annotations of grammatical properties and poetic features related to sound devices.

## Size:

650 561 rhyme pairs and their grammatical, phonological and positional features described below

## Formats:

- rhyming\_dictionary\_XML.zip: The compressed file contains the XML version of the rhyming dictionary. The file must be unzipped after downloading.
- rhyming_dictionary\_TSV.zip: The compressed file contains the rhyming dictionary in a tabular format. This version is suitable for use in spreadsheet software. The file must be unzipped after downloading.
- rhyming\_dictionary\_SQLite.zip: The compressed file contains the SQLite version of the rhyming dictionary. This version is suitable for use in database systems. The file must be unzipped after downloading.
- rhyming\_dictionary\_PDF: The folder contains the PDF version of the rhyming dictionary in several files. This version is suitable for manual reading.

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

## Columns of the TSV and SQlite files:

- `id_rhyme_pair`: id number of the rhyme pair
- `wordform1`: one rhyming word in the rhyme pair
- `wordform2`: the other rhyming word in the rhyme pair
- `lemma1`: lemma of wordform1
- `lemma2`: lemma of wordform2
- `pos1`: part of speech of wordform1 ([Universal Dependencies](https://universaldependencies.org/))
- `pos2`: part of speech of wordform2
- `msd1`: morphosyntactic features of wordform1 ([Universal Dependencies](https://universaldependencies.org/))
- `msd2`: morphosyntactic features of wordform2
- `num_syll1`: syllable number of wordform1
- `num_syll2`: syllable number of wordform2
- `phon_type1`: type of vowels in wordform1
   - `low`: only back vowels in the word
   - `high`: only front vowels in the word
   - `mixed`: front and back vowels in the word
- `phon_type2`: type of vowels in wordform2
- `phon_struct1`: phonological representation of wordform1
   - `c`: consonant
   - `b`: short back vowel
   - `B`: long back vowel
   - `f`: short front vowel
   - `F`: long front vowel
- `phon_struct_2`: phonological representation of wordform2
- `word_id1`: ID of wordform1
- `word_id2`: ID of wordform2
- `between_rhymes`: number of lines rhyming with the rhyming pair between the two words of the rhyming pair
- `distance`: distance of the two rhyming words 
- `author`: author of the poem in which the rhyme pair occurs
- `title`: title of the poem in which the rhyme pair occurs 
- `stanza_id`: ID of the stanza in which the rhyme pair occurs 
- `poem_id`: ID of the poem in which the rhyme pair occurs 
- `url`: URL of the poem in which the rhyme pair occurs

## Fields of the PDF files:

__rhyming\_word\_1 – rhyming\_word\_2__ (lemma1, part\_of\_speech\_1 – lemma2, part\_of_speech\_2), Author: _The first 4 words of the poem title_ serial number of the stanza (distance of the two rhyming words, number of lines rhyming with the rhyming pair between the two words of the rhyming pair)

## Licence:

The content of the rhyming dictionary is licensed under the [CC BY-NC-ND](https://creativecommons.org/licenses/by-nc-nd/4.0/) license.

## Creator:

Anonymized for peer review



