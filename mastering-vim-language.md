# Mastering The Vim Language

> Typing is not the bottleneck

> Vim's killer feature is the language it provides for making changes

## Syntax of the language
**Verb + Noun**

`d` for delete, `w` for word, combine to be "delete word"

> Commands are **Repeatable & Undoable**

## Verbs in Vim

- d => **Delete**
- c => **Change** (delete and enter insert mode)
- > => **Indent**
- v => **Visually select**
- y => **Yank** (copy)

## Nouns in Vim

- w => **word** (forward by a "word")
- b => **back** (back by a "word")
- 2j => down 2 lines

### Nouns in Vim -- Text Objects

These nouns works by combining them with *verbs*

- iw => "inner word" (works from anywhere in a word).
- it => "inner tag" (the contents of an HTML tag)
- i" => "inner quote"
- ip => "inner paragraph"
- as => " a sentence"

## Nouns in Vim -- Parameterized Text Objects

- f, F => "find" the next character (inclusive)
- t, T => "find" the next character (exclusive)
- / => Search (up to the next match)

## Combinatorics of Commands

5 operators + 10 motions
+ 5 operators * 10 text objects
+ 5 operators * 35 characters * 4 (for `f`, `F`, `t`, `T`)
+ 5 operators * ~100 (for `/`)

> **2000** distinct commands based on memorizeing ~30 key mappings (that are very memorable)

## Tips for Mastering The Vim Language

> The "dot" command

- Use the more general text object (`iw` rather than `w` even if at beginning of word)
- Prefer text objects to motions when possible
- Repeat.vim for plugin repeating

## Relative Numbers


