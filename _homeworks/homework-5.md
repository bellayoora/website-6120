---
layout: page
title: homework 5
permalink: /homework-5/
description: word embeddings
nav: true
hw_pdf: assignment-5.pdf
assigned: february 20
due_date: march 6
horizontal: false
---

<hr style="border:2px solid gray">
#### mastering map reduce
-----

Review the homework in this [pdf file]({{ site.baseurl }}/assets/pdf/assignment-3.pdf). Remember that reading resources can be found in the [syllabus]({{ site.baseurl }}/syllabus).

Word Vectors are often used as a fundamental component for downstream NLP tasks, e.g. question answering, text generation, translation, etc., so it is important to build some intuitions as to their strengths and weaknesses. Here, you will explore two types of word vectors: those derived from co-occurrence matrices, and those derived via GloVe.

**Note on Terminology**: The terms "word vectors" and "word embeddings" are often used interchangeably. The term "embedding" refers to the fact that we are encoding aspects of a word's meaning in a lower dimensional space. As Wikipedia states, "conceptually it involves a mathematical embedding from a space with one dimension per word to a continuous vector space with a much lower dimension".



-----
#### data and starter kit
-----

We will be using the IMBD dataset today.

```python
from datasets import load_dataset
imdb_dataset = load_dataset("stanfordnlp/imdb")
```

You will need [the data](https://course.ccs.neu.edu/cs6220/fall2023/homework-3/). If you are using Colabs (not a requirement), you would need a Google account.

<center>
<img 
  src="https://thehubbackend.com/media/49573-0_QxsWlMTDGmTebavF.jpg"
  width="500" height="auto">
</center>
<br>

Here are the starter kits that you might find useful.

* Document templates can be either [Overleaf TeX File](https://www.overleaf.com/read/gbwryydmdjhv) or [DOCX File](https://docs.google.com/document/d/1Q8fpJo-gF_L0_TwUdw5E7x7faOAStK4n). When you've compiled/finishe
d writing, **download the PDF** from Overleaf/Google and upload it to the submission link. 

* Upload your processed `output.txt` file in the specified format in the [homework questions]({{ site.baseurl }}/assets/pdf/assignment-3.pdf)

* To help you get started, you may find that this [Colaboratory Link](https://colab.research.google.com/drive/1dAqxrOEqrvlqhCJ2jwKX4UrDlNNACWC7?usp=sharing) is useful. In order to submit, you'll need to Download the file as a `*.ipynb` file (Under **File** &rarr; **Download** &rarr; **Download .ipynb**.)

<br>
#### submission instructions

* Commit your `*.py` or `*.ipynb` (either is fine as long as they are commented appropriately), `output.txt`, and `name-submission-3.pdf` to that 
repository and provide the URL via [Gradescope](https://www.gradescope.com/courses/690988/assignments/4010650) before 5pm, Thursday, February 8.

* Make sure that you have documented your code with comments so that the TA can have an easier time understanding your logic. This will, in some cases, result in at least partial credit.

* Include a diagram of your pipeline description in your writeup.

* Include in your writeup the recommendations for the users with following user IDs: 924, 8941, 8942, 9019, 9020, 9021, 9022, 9990, 9992, 9993.

* We will be checking for plagiarism, comparing code that is too similar to classmate or past class alumni homework. This will automatically result in zero credit.


