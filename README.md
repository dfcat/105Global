# 105Global
Shared translated metadata for DFCAT G105/F105 supports multi-language.

```ko``` / ```en``` / ```jp``` / ```cn```

# Contribution
Anyone want to contribute can participate in translation by **PULL REQUEST**. 

This project is in 3 stages.

# Stage1 : Translator
Translator ```f105.**.js```

Using display functions. Fast but some informations(growInfo, status, item explain, buffer only, item flavor text) cannot be translated. This file is just 579 lines now. 

In this stage, we translate **set name**, **item name**, **dungeon name**, **boss name**, **tags**, and **ui** (a.k.a. base info).

Edit values in each language file.
(**DO NOT EDIT KEY!** JSON is key-value pair structed format. left-side is key, and right-side is value. "key": "value". Just edit right-side of colon(:).)

# Stage2 : Metadata
item metadata ```meta.**.js```

Translate missing informations in **Stage 1** (growInfo, status, item explain, buffer only, item flavor text. aka detail info).

Just edit values of these keys, and leave others. **BE CAREFULL!** It may cause disorder


# Stage3 : Merge
Translator ```f105.**.js```
item metadata ```meta.**.js```
set metadata ```set.**.js```

After Stage 1 & 2 completed, move base info from **Translator** to **metadatas**

Translators focus to ui and metadata is translated in native to accelerate performance bypass display function.

There is no difference in UX excepts performance from Stage 2. 


# Translate README.md
If you want to translate this file, add translated lines below each line.

```
i.e
English line~~~
Japanese line~~~
Chinese line~~~
```

