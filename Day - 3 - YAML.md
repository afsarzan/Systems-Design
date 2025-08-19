# YAML Ain't Markup Language

* .yaml( official extention ) or .yml ( historical reason) both are file extention

* Yaml is a data serialisation language 
* YAML avoids {}, [],,, and " in most cases.
* Fewer chances of syntax errors like a trailing comma in JSON.
* Comments
* Anchor and Aliases → re-usability

---

## Basic YAML Syntax
Data Types
1. We Specify Data Types by Line Separation and Indentation.
2. YAML is case sensitive.
3. indentation: Some rules are fixed some are not

* | use pipe for multi line
```
description: |
    This is a multi-line strng.
    Line breaks are preserved.
    Indentation is important.
```
* anchor imprements DRY
* **&** use to create variable and **<<:** used to implement , just like include funtion in php or var(--name) in css
```
person: &personObj
    age: 29
    superhero: *myName

magical Person:
<<:
*personObj
```
