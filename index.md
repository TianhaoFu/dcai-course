---
layout: page
title: Introduction to Data-Centric AI
nositetitle: true
subtitle: IAP 2023
description: >
  The first-ever course on data-centric AI. Learn how you can train better ML
  models by improving the data.
thumbnail: /static/assets/thumbnail.png
---

Typical machine learning classes teach techniques to produce effective models for a given dataset. In real-world applications, data is messy and improving models is not the only way to get better performance. You can also improve the dataset itself rather than treating it as fixed. **Data-Centric AI** (DCAI) is an emerging science that studies techniques to improve datasets, which is often the best way to improve performance in practical ML applications. While good data scientists have long practiced this manually via ad hoc trial/error and intuition, DCAI considers the improvement of data as a systematic engineering discipline.

This is the first-ever course on DCAI. This class covers algorithms to find and fix common issues in ML data and to construct better datasets, concentrating on data used in supervised learning tasks like classification. All material taught in this course is highly practical, focused on impactful aspects of real-world ML applications, rather than mathematical details of how particular models work.  You can take this course to learn practical techniques not covered in most ML classes, which will help mitigate the “garbage in, garbage out” problem that plagues many real-world ML applications.

![Flawed Data](/static/assets/flawed_data.png)

<p class="small center">Inspired by <a href="https://xkcd.com/2494/">XKCD 2494</a> &ldquo;Flawed Data&rdquo;</p>

{% comment %}
# Registration

Sign up for the IAP class by filling out this [**registration form**](https://forms.gle/iYB9bQeDgwVySpCp8).
{% endcomment %}

# Syllabus

<ul>
{% assign lectures = site['lectures'] | sort: 'date' %}
{% for lecture in lectures %}
    <li>
    <strong>{{ lecture.date | date: '%-m/%d/%y' }}</strong>:
    {% if lecture.ready %}
        <a href="{{ lecture.url }}">{{ lecture.title }}</a>
    {% else %}
        {{ lecture.title }}
    {% endif %}
    </li>
{% endfor %}
</ul>

Video recordings of the lectures are available <a href="https://www.youtube.com/watch?v=ayzOzZGHZy4&list=PLnSYPjg2dHQKdig0vVbN-ZnEU0yNJ1mo5">on YouTube</a>.

Each lecture has an accompanying [lab
assignment](https://github.com/dcai-course/dcai-lab), a hands-on programming
exercise in Python / Jupyter Notebook.

{% comment %}
You can work on these on your own, in
groups, and/or in office hours. This is a not-for-credit IAP class, so you
don't need to hand in homework.
{% endcomment %}

# General information

{% comment %}
**Dates**: Tuesday, January 17 -- Friday, January 27, 2023<br>
**Lecture**: [6-120](https://whereis.mit.edu/?go=6), 1pm--2pm<br>
**Office hours**: [2-132](https://whereis.mit.edu/?go=2), 3pm--5pm (every day, after lecture)
{% endcomment %}

**Staff**: This class is co-taught by [Anish](https://www.anish.io/), [Curtis](https://www.curtisnorthcutt.com/), [Jonas](https://people.csail.mit.edu/jonasmueller/), [Cody](https://www.codycoleman.com/), [Ola](https://olazytek.mit.edu/), and [Sharon](https://twitter.com/realSharonZhou).<br>
**Questions**: Join `#dcai-course` on this [Slack](https://cleanlab.ai/slack/).<br>

# Prerequisites

Anyone is welcome to take this course, regardless of background. To
get the most out of this course, we recommend that you:

- Completed an introductory course in machine learning (like [6.036 / 6.390](https://introml.mit.edu/)). To learn this on your own, check out [Andrew Ng's ML course](https://www.coursera.org/learn/machine-learning), [fast.ai's ML course](https://course.fast.ai/), or [Dive into Deep Learning](https://d2l.ai/).
- Are familiar with Python and its basic data science ecosystem (pandas, NumPy, scikit-learn, and Jupyter Notebook). To learn this on your own, check out [Jupyter Notebook 101](https://github.com/fastai/fastbook/blob/master/app_jupyter.ipynb), [Introduction to Pandas](https://walkwithfastai.com/Pandas), and [Python for Data Analysis](https://www.coursera.org/projects/python-for-data-analysis-numpy).

# Beyond MIT

We've also shared this class beyond MIT in the hopes that others may
benefit from these resources. You can find posts and discussions on:

- [r/MachineLearning](https://www.reddit.com/r/MachineLearning/comments/1194wm0/p_mit_introduction_to_datacentric_ai/)
- [r/learnmachinelearning](https://www.reddit.com/r/learnmachinelearning/comments/1194vsn/mit_introduction_to_datacentric_ai/)
- [Twitter](https://twitter.com/anishathalye/status/1628437244464992256)
- [LinkedIn](https://www.linkedin.com/pulse/teaching-first-data-centric-ai-course-mit-curtis-northcutt/)
- [Lobsters](https://lobste.rs/s/qtaba8/mit_introduction_data_centric_ai)

## Acknowledgements

We thank Elaine Mello / [MIT Open Learning](https://openlearning.mit.edu/) for
making it possible for us to record lecture videos, Kate Weishaar / [MIT Office
of Experiential Learning](https://elo.mit.edu/) for supporting this class, and
Ashay Athalye / [MIT SOUL](https://mitsoul.org/) for editing the lecture
videos.

---

<div class="small center">
<p><a href="https://github.com/dcai-course/dcai-course">Source code</a>.</p>
<p>Licensed under CC BY-NC-SA.</p>
<p>See <a href="/license/">here</a> for contribution &amp; translation guidelines.</p>
</div>
