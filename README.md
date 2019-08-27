# ngrams
pseudo-random text generator using ngram models

```
Generate text using randomized word ngrams from standard input.

positional arguments:
  n                     the number of words to consider simultaneously when
                        generating text.
  min_length            each iteration will be retried until the minimum
                        length (in words) is reached.
  max_length            length (in words) at which to cease generating text if
                        no end token found. Note: the [min, max] length range
                        is inclusive.
  iterations            The number of text snippets to generate.

optional arguments:
  -h, --help            show this help message and exit
  --text_files TEXT_FILES [TEXT_FILES ...]
                        optional list of files to read in lieu of stdin.
  --start_token START_TOKEN
                        predetermined first word of output text
  --end_token END_TOKEN
                        delimeter at which a given text generation iteration
                        stops; not included in generated text. Must be
                        distinct from the start token.
  --seed SEED           seed to control random text generation
  --ngram_model_file NGRAM_MODEL_FILE
                        if a file path ending in .ngrams is specified, the
                        ngram model will be deserialized FROM the provided
                        path (if it exists); otherwise, it will be treated as
                        an output parameter, and the model will be serialized
                        TO the provided path.
```
