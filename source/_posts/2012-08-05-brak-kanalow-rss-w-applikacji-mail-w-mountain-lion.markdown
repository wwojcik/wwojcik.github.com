---
layout: post
title: "Brak kanałów RSS w applikacji Mail w Mountain Lion"
date: 2012-08-05 10:56
comments: true
categories: [MacOS]
tags: [MacOS]
---
Po aktualizacji MacOS do Mountain Lion z aplikacji Mail zniknął mi czytnik RSS.

Jak odnaleźć subskrybowane kanały:
{% codeblock %}
cd ~/Library/Mail/V2/RSS/
find . -name "Info.plist" -exec grep -A 1 Feed {} \; | grep string | sed 's/^[^>]*>//' | sed 's/<[^>]*>$//'
{% endcodeblock %}

Otrzymujemy listę subskrybowanych kanałów, którą możemy wkleić np do  Reeder lub Google Reader.
