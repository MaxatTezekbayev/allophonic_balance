### Prerequisites:
1) Download and process IWSLT'14 dataset via script [prepare-iwslt14.sh](https://github.com/facebookresearch/fairseq/blob/main/examples/translation/prepare-iwslt14.sh) used in Fairseq repo
2) Clone [cmudict-ipa repo](https://github.com/menelik3/cmudict-ipa). It is needed for getting possible onsets used for syllabification of phonemes.

### Scripts:
1) **1_generate_phonemes_for_iwslt14.ipynb**: Script converts text into phonemes via [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P) transformer-based model.
2) **2_main_code.ipynb**: Breaks phonemes into syllables and counts occurrences of each phone in each context, and normalizes the counts to calculate weighted phonetic coverage of a given text.

 
