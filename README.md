# Regex-for-HB
Useful regex for HB

[^\u0590-\u05FF]+([\u0590-\u05FF]){2}[^\u0590-\u05FF]
* Find 2 letter words

([^\u0590-\u05FF]{1}[\u0590-\u05FF]+|[\u0590-\u05FF]+[^\u0590-\u05FF]{1})
* Word boundries

([בהוכלמש][\u05B0-\u05C3]*)+[-‑]?\w+
* Find prefixed preposition (with niqqud?) with hyphen

[\u0590-\u05FF]*[ךםןףץ][\u0590-\u05FF]+
* final forms in the middle of the word

["״][(\u0590-\u05FF)(\w)]+(\s+[(\u0590-\u05FF)(\w)]+)?["״][\s\.\,\:]
* Find quotes

"(?!([(\u0590-\u05FF)(\w)]+(\s+[(\u0590-\u05FF)(\w)]+)?[״][\s\.\,\:]))
* Find mismatching quotes
