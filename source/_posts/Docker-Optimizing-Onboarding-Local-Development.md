---
title: Docker - Optimizing Onboarding & Local Development
date: 2022-11-27 09:43:40
author: Yoseph Alabdulwahab
categories: [articles]
draft: false
---
<span style="display: none;">
    Hook - Describe the problem statement

    We can use docker to solve this problem
    - different implementations
    - chosen implementation

    Short comings of docker:
    - File mounting
    - Synchronization

    Encapsulating the last bit of manual effort with tasks
    - Using vscode task / mvn / ant / grunt

    Mini tutorial
</span>

I recently got back from QCon in San Fransico and had the pleasure to interact with so many engineers in every part of this industry. It seemed that so many companies attending the conference had a similar problem. They have a big painful monolith running the majority of their services while slowly migrating to microservices. In the meantime, setting up a new machine is a multi day labourous effort, and daily development is painful at best. This begs the question, do we stay complacent with the hope of our migration to happen quicker, or can we do a little bit of optimization and enhance the onboarding and daily development experience?

## What can we do?
The core of the problem is that many older frameworks are big puzzles that require all sorts of dependencies to be installed in a particular way and configuration can be too easly altered affecting the development environment. Additionally when something changes and breaks the local environment, debugging is akin to ghost hunting. Wouldn't it be nice to simplify the setup process to a simple git pull and a start command. That's where Docker comes in.

