---
date:
  created: 2025-04-17
draft: false
---

# New Website with Blog and Minor RST-Tace Update

Today, this small website sees the light of day. :partying_face:

It is supposed to serve as a space for documenting personal projects, thoughts on the status or development of the ADAS/AD industry, machine learning, computer science as a whole, and other topics of interest (e.g., astronomy).

In the upcoming time, I will expand this space with further contributions. Let's see how it develops in the future. :smile:

But first, I want to announce the a minor update of [RST-Tace](https://github.com/tkutschbach/RST-Tace):

<!-- more -->

---

[RST-Tace](https://github.com/tkutschbach/RST-Tace) is a tool in the wider field of *natural language processing and analysis* — more specifically, in the field of *Rhetorical Structure Theory*. It was created during a research project by [ShujunW](https://github.com/ShujunW) and published at the [Discourse Relation Parsing and Treebanking (DISRPT)](https://sites.google.com/view/disrpt2019/) workshop of the NAACL conference in Minneapolis in 2019.

Now, six years old and initially developed and tested with [Python 3.6](https://www.python.org/downloads/release/python-360/), it was in need of a small update. [Pandas](https://pandas.pydata.org) was updated to [version 2.x](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) in the meantime, which introduced some changes in how dataframes are handled.

While the initially published [version 0.1.0](https://github.com/tkutschbach/RST-Tace/releases/tag/v0.1.0) of [RST-Tace](https://github.com/tkutschbach/RST-Tace) still works perfectly fine when using the CLI as the output interface, the CSV output threw an error:

The functionality of outputting a CSV when comparing two sets of multiple RST trees relied on the now-deprecated `dataframe.append()` function.

With [version 0.1.1](https://github.com/tkutschbach/RST-Tace/commit/00ab7e5dae50cb2402a1b2d9e9f38b50c1c82e78) (tested with [Pyhon 3.13.2](https://www.python.org/downloads/release/python-3132/)), this issue has now been fixed.

If you found another issues or if you have a feature request for [RST-Tace](https://github.com/tkutschbach/RST-Tace), feel free to add an [issue](https://github.com/tkutschbach/RST-Tace/issues).

Thank you very much! ~
