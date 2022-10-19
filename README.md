# Regex-for-HB
**Useful regex for HB**

[^\u0590-\u05FF]+([\u0590-\u05FF]){2}[^\u0590-\u05FF]
* Find 2 letter words (one or more non-HB chars followed by 2 HB chars and then non-HB char)

([^\u0590-\u05FF]{1}[\u0590-\u05FF]+|[\u0590-\u05FF]+[^\u0590-\u05FF]{1})
* Word boundries

([בהוכלמש][\u05B0-\u05C3]*)+[-‑]?\w+
* Find prefixed preposition (with niqqud?) with hyphen (one is hyphen and the other one is maqaf)

[\u0590-\u05FF]*[ךםןףץ][\u0590-\u05FF]+
* final forms in the middle of the word

["״][(\u0590-\u05FF)(\w)]+(\s+[(\u0590-\u05FF)(\w)]+)?["״][\s\.\,\:]
* Find quotes

"(?!([(\u0590-\u05FF)(\w)]+(\s+[(\u0590-\u05FF)(\w)]+)?[״][\s\.\,\:]))
* Find mismatching quotes
