You are a lexical data generator. Produce dictionary-style JSON entries following the **exact structure** and formatting shown below.

Each entry should describe one English word in detail.

#### ✅ **Requirements:**

1. **Follow this JSON structure exactly:**

   ```json
   {
     "id": "unique_id",
     "word": "Word",
     "partOfSpeech": "part_of_speech",
     "shortExplanation": "short one-line meaning",
     "longExplanation": "longer and more detailed meaning or definition",
     "links": [
       {
         "url": "https://valid-link-to-wikipedia-or-reputable-vocabulary-site",
         "type": "wikipedia",
         "label": "Wikipedia: [Word]"
       }
     ],
     "pronunciation": "IPA notation (e.g. /juːˈbɪkwɪtəs/)",
     "examples": [
       {
         "sentence": "An example sentence using the word naturally.",
         "context": "Thematic or usage context (e.g. Technology, Literature, Business)"
       },
       {
         "sentence": "Another different example of the word.",
         "context": "Different context"
       }
     ],
     "synonyms": [
       {
         "word": "Synonym1",
         "coreMeaning": "Concise meaning or distinction",
         "translations": {
           "en": "...",
           "es": "...",
           "ru": "...",
           "zh": "...",
           "fr": "...",
           "de": "...",
           "ja": "...",
           "pt": "...",
           "ar": "...",
           "hi": "...",
           "ko": "...",
           "it": "...",
           "nl": "...",
           "sv": "...",
           "no": "...",
           "tr": "...",
           "pl": "...",
           "uk": "...",
           "cs": "...",
           "fa": "..."
         }
       }
     ],
     "antonyms": [
       {
         "word": "Antonym1",
         "coreMeaning": "Concise opposite meaning",
         "translations": {
           "en": "...",
           "es": "...",
           "ru": "...",
           "zh": "...",
           "fr": "...",
           "de": "...",
           "ja": "...",
           "pt": "...",
           "ar": "...",
           "hi": "...",
           "ko": "...",
           "it": "...",
           "nl": "...",
           "sv": "...",
           "no": "...",
           "tr": "...",
           "pl": "...",
           "uk": "...",
           "cs": "...",
           "fa": "..."
         }
       }
     ],
     "frequency": 1–10 scale of how commonly the word appears in English,
     "translation": "Native-language translation in Russian (ru)",
     "imageUrl": "https://a-valid-image-link-related-to-the-word",
     "translations": {
       "en": "Word",
       "ru": "...",
       "es": "...",
       "zh": "...",
       "fr": "...",
       "de": "...",
       "ja": "...",
       "pt": "...",
       "ar": "...",
       "hi": "...",
       "ko": "...",
       "it": "...",
       "nl": "...",
       "sv": "...",
       "no": "...",
       "tr": "...",
       "pl": "...",
       "uk": "...",
       "cs": "...",
       "fa": "..."
     }
   }
   ```

2. **Translation requirement:**
   Provide accurate translations for **20 major world languages**:
   English (en), Spanish (es), Russian (ru), Chinese (zh), French (fr), German (de), Japanese (ja), Portuguese (pt), Arabic (ar), Hindi (hi), Korean (ko), Italian (it), Dutch (nl), Swedish (sv), Norwegian (no), Turkish (tr), Polish (pl), Ukrainian (uk), Czech (cs), Persian/Farsi (fa).

3. **Links must be valid:**

   * Preferably from Wikipedia, Oxford Learner’s Dictionary, Merriam-Webster, or Cambridge.
   * Each link must lead to a real, existing page relevant to the word.

4. **Image URL:**
   Use a valid, copyright-safe Unsplash image URL that visually represents the concept.

5. **Style:**

   * All text must be natural, clear, and lexically correct.
   * Definitions should be factually accurate and stylistically neutral.
   * Avoid filler or vague language.

6. **Example contexts:**
   Always use realistic, everyday examples from different domains (e.g., technology, literature, education, social life, etc.).

For words iterate in the current directory for TXT files. Place otput into the same directory with same names as input file, but with a .json extension.
Do iteratively file by file. Process everything with the model. Don't generate code to acomplish the task.