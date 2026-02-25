---
title: "TIL: creating an actual website"
date: 2026-02-25
categories: til
---

i'm on my day 2 of social media detox and that has increased the amount of time my dmn stays active and so today i got an idea about creating an actual website. 

an actual friendly bets website that i can share with friends.

they will
1. log in with google
2. create or join bets
3. place bets

this requires hosting the website, integrating google authorisation, needing a database. i asked Gemini 3.1 Pro about the steps to do this. it said i could use supabase for database and vercel for hosting. 

i started visual studio code, pressed the codex extension and asked it to build. it coded continuously for 15 minutes and gave me a bunch of files. 

then i had to -
1. start a supabase project
2. start a google cloud console project and integrate the keys for google account login.
3. run the version locally to test and debug.

the first problem i encountered was that when pressing login with google, the website would load for a bit and then say that the supabase project url wasn't responding. the reason for this it turned out after trying multiple things suggested by gpt 5.2 was that my dns was blocking it for some reason. 

once that was solved, i could see the basic homepage.
