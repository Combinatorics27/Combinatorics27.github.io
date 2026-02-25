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

then i had to test this locally. so i had to download node.js and put in the supabase api keys and then do the local testing. 

the first problem i encountered was that when pressing login with google, the website would load for a bit and then say that the supabase project url wasn't responding. the reason for this, it turned out, after trying multiple things suggested by gpt 5.2 was that my wifi dns was blocking it for some reason. 

once that was solved, i could see the basic homepage.

but then the create bet button didn't work. it did nothing - didn't add to the database, didn't throw up an error. (now what i was doing was using gpt 5.2 on the web as an auditor or second opinion of sorts. codex was the primary, but for some issues, i referred to gpt 5.2 on the web instead.) and then i told it the issue and it threw a bunch of diagnosis steps - do this, if it works, then try the next step to check if thats the issue and so on.

it took time. and patience. and it was frustrating at times. 

but it was solved. but then the current bets section would show nothing. it was a coding error in the sql code which fetched data from the supabase database. then the ai solved it. 

and so i had a running website locally. the next step was to deploy it through vercel so that my friends could use it as well. 

so i downloaded the github connector. then created a repository and pushed the code form my laptop to github. 

then connected github and vercel and deployed the website. and it failed. so i copied the error and gave it to codex. it changed a file. i committed and pushed the new files to github. then redeployed on vercel. errors again. so back to codex. commit and push. redeploy. errors. codex. commit and push. redeploy. errors. codex. push. redeploy. errors. codex. push. redeploy.
