# Project Honoka l10n repository
Public repo for translations for Project Honoka

There are **two** types of files to translate:

* Docs: Documentations or similars which are made and written in Markdown format. Please, respect the format
* Strings: JSON Files containing the strings to use

Sample JSON Data:

```json
{
    "COMMON_STRING":"Hello World",
    "HELLO_WORLD": "Ciao mondo"
}
```

The left one (`COMMON_STRING`) **MUST** be left as is, meanwhile the right one (`Hello World`) is the string which you need to edit. Make sure that you follow the JSON rules about the use of commas.

## I want to add a new language. Can I?

Of course. Copy the English (or other source file) and start to translate it. 

File names **MUST** follow this format: 

* `Docs`: `<lang>_api.md`
* `Strings`: `<lang>.json`

where lang is the name of the language using **ONLY** two chars like `en` (English) or `ja` (Japanese).

## Updates

I was planning to make a Discord Server where we may discuss together and easily about how to translate the various strings/documentations. For now you may just read the file `<lang>.log` inside the `reports` folder to see which entries had been added.