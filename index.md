---
title: Pixie the Elf writes Perl
description: >
  Pixie the Elf is a cheerful Perl hacker at the North Pole. This page
  collects all of her Perl Advent calendar stories in one place.
image: /pixie-the-elf.png

---

<p class="pixie-home-link">
  <a href="https://perlhacks.com/">Home</a>
</p>

# Pixie the Elf writes Perl

<img
  src="{{ '/pixie-the-elf.png' | relative_url }}"
  alt="Pixie the Elf, a young red-haired elf working on a laptop in Santa's office at the North Pole"
  class="pixie-hero">

Over the last few years I've written a few blog posts for Perl-related
Advent calendars. Recently, they have been about Pixie the Elf (whose
parents had strange ideas about names).

I thought it would be a good idea to start to collect a list of these
posts, so I can remember where and when they were posted.

{% assign posts = site.data.posts | sort: 'date' %}
| Year | Date | Site | Title | Subject |
|------| ---- | ---- | ----- | ------- |
{% for post in posts -%}
| {{ post.date | date: "%Y" }} | {{ post.date | date: "%-d %b" }} | {{ post.site }} | [{{ post.title }}]({{ post.url }}) | [{{ post.subject.name }}]({{ post.subject.url }}) |
{% endfor %}

---

Hi, I'm Dave and I wrote the blog posts about Pixie the Elf. I've been working
in Perl and various web technologies for approaching forty years. If you think
that [any of my skills](https://davecross.co.uk/services/) could be of interest
to you, then why not [get in touch](https://davecross.co.uk/contact/)?
