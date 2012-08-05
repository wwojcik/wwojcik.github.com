---
layout: post
title: "Zmiany w Heroku"
date: 2012-08-01 23:54
comments: true
categories: Heroku
tags: Heroku
---
Dzisiaj Heroku wydało free Heroku Postgres `dev` plan, który będzie zastępował Shared Database.
W otrzymanym mailu od Heroku w tej sprawie można przeczytać:
{% blockquote %}
Because of the significant stability and feature improvements in this new service, we are deprecating Shared Databases and will begin automatically migrating databases gradually over the month of August, beginning on August 9. Prior to your migration, we will send you an e-mail notice with the exact date & time.


If you have unusual circumstances and require more time before the auto migration occurs, you can request an extension to your automatic migration date. We will do our best to honor all requests.


The new `dev` plan offers many advantages, including Postgres 9.1 with schemaless SQL, direct psql access, data clips, and a web management interface. It also imposes a hard limit of 10,000 rows, comparable to the 5mb limit you have now. Check the size of your existing database if you are unsure if you are over the limit.


We strongly encourage you to migrate the database(s) yourself. By doing this you will have complete control over when the migration and associated downtime occur. As an added incentive, we will increase the row-limit from 10,000 to 14,000 rows if you migrate yourself prior to 12pm PDT August 9. 


Don’t hesitate. You can begin right now by provisioning a dev database.
{% endblockquote %}
