# Translation with Glossary

## Problem

You are given a glossary containing individual Portuguese words and their English equivalents.  
You are also given a sentence represented as a list of Portuguese words.

Your task is to translate the sentence word by word using the glossary.  
If a word does not exist in the glossary, leave it unchanged in the output.

---

## Notes

- The translation must preserve the original word order.
- The search should be **case-insensitive**.
- If a word is not found in the glossary (even after normalizing case), it must be kept unchanged.
- You may assume all words are space-separated and contain no punctuation.

---

## Input

- `glossary`: A list of pairs, where each pair contains a Portuguese word and its English translation.
- `sentence`: A list or array of words representing a sentence in Portuguese.

---

## Output

- A list or array of words representing the sentence translated into English.
- Each Portuguese word must be replaced by its English equivalent if it exists in the glossary.

---

## Example 1

### Input

```
glossary = [
  ["o", "the"],
  ["livro", "book"],
  ["está", "is"],
  ["sobre", "on"],
  ["a", "the"],
  ["mesa", "table"]
]

sentence = ["O", "livro", "está", "sobre", "a", "mesa"]
```

### Output

```
["the", "book", "is", "on", "the", "table"]
```

---

## Example 2

### Input

```
glossary = [
  ["chave", "key"],
  ["porta", "door"]
]

sentence = ["A", "chave", "estava", "embaixo", "da", "porta"]
```

### Output

```
["A", "key", "estava", "embaixo", "da", "door"]
```
