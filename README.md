# Poster Py

A script that can autonomously post messages to a number of social networks.

## Desription

The user creates a list of posts saveid in some kind of a "databse". It can be a plain json file or an sqlite database.
The user schedules the process to run at some interval. (The scheduleing can be done externally by the Windows scheduler or crontab).
On each run the scripts takes the next item and posts in on one or more social networks.

The items then can be placed at the end of the queue or marked as "done". (This should be configurable.)

The user should be able to add/edit/remove items from the queue.

The user should be able to mark items to be "live" or "on-hold". The "on-hold" items are skipped or rescheduled
when their turn comes. (This won't change thir status though, just so the order won't change.)

The user should be able to reorder the items.

The system can have a CLI interface, a GUI (e.g. using Tk), a self-hosting web interface. It could also have
multiple interfaces.

## Social networks:

in order of interest:

1) LinkedIn - on a company page managed by the user. (e.g. https://www.linkedin.com/company/code-maven-world )
2) LinkedIn - on the personal account. (e.g. https://www.linkedin.com/in/szabgab/ )

3) Facebook - a Facebook page owned or managed by the user.
4) Facebook - the personal wall of the user.

5) Twitter

## Posts

Each post might include free text, one or more links to external resources (e.g. YouTube videos, post on a web site)
They should be able to include hash-tags, e.g. #python and references to people. ( @username ).

Specific social networks might behave differently.

## Insttructions

We need to include clear instructions on how to set up the system for individual.
