# JavaScript Usage Guide

*Jake Johnson's Guide to Cleaner Code*

*(NOTE: This guide contains recommendations. Some of them really matter. Many do not. In a job setting prefer the in-place standards when talking about things like camelCase versus snake_case and any other items that are opinions and not best practices.)*

# Table of Contents

[Rules](https://github.com/ofalltrades/language-usage-guides/blob/master/javascript/javascript.md#Rules)

[Recommendations](https://github.com/ofalltrades/language-usage-guides/blob/master/javascript/javascript.md#Recommendations)

[Reasoning](https://github.com/ofalltrades/language-usage-guides/blob/master/javascript/javascript.md#Reasoning)

# Rules

1. There is only one rule: Do what is best for the **team**, and *then* do what is best for the code, **unless** the **team** is using **actual bad practices**, meaning no-no code, aka **dangerous code.**

# Recommendations

## Naming

```js
var var_is_bad = 'Prefer let or const.';
let let_is_ok = 'Use let for variable';
const const_is_best = 'Prefer top-level objects and literals that are immutable';

const badVariableName = 'This variable name is slightly inferior.';
const good_variable_name = 'This is a slightly more readable variable name.';

const _bad_variable_name = 'Do not use _ (underscores) or $ as prefix or suffix';
const $bad_variable_name = 'Do not use _ (underscores) or $ as prefix or suffix';
const bad_variable_name_ = 'Do not use _ (underscores) or $ as prefix or suffix';
const bad_variable_name$ = 'Do not use _ (underscores) or $ as prefix or suffix';

const prefer_explicit_trailing_semicolons = 'in a work setting where semicolons are not managed by some sort of linting tool';
const i_personally_omit_semicolons = 'and prefer having Prettier and-or like-tools to manage semicolon insertion.'

const bd_vr_nm = true;
const better_variable_name = true; // Prefer clarity over terseness.  

const prefer_no_trailing_commas_in_lists = ['because I think it is weird',];
```

# Reasoning

## People

1. Prefer what is best for the team, not yourself.

## Naming

1. Refrain from using `_` or `$` as the prefix or suffix of a name. This includes prefixing function names with `_` to indicate accessibility. They are for those non-human and were not intended to be used in this manner in JavaScript.

2. Prefer naming using snake_case, words separated by `_`. This is easier for most English-speaking humans to read and because it reflects separation of words as we expect in prose. This is better than camelCase. Prefer clarity over dogma.

## Numbers

1.

## Booleans

## Arrays

## Objects

## Strings

## Statements

### Semicolons

In general prefer ending statements with an explicit `;`, especially in a work setting... unless everyone uses something like Prettier and that it formats on save. This will manage semicolons for you, and you can feel nice and modern. In all other cases, make those `;`s explicit. I personally recommend never omitting semicolons in a work environment, not pretty but safer. In my personal project I omit. At work, I don't.

## Functions

## Class(less)

## Purity & Immutability

## Dates

## JSON

## Testing

## The English Language

## References & Further Reading

I have no original ideas. I'm not sure anyone does. I stole this material from:

* Douglas Crockford
* Others
