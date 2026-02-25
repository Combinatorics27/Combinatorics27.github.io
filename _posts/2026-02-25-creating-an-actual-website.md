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

then it worked. i could see the preview. deployment successful. 

i copied the domain name https://friendlybets-three.vercel.app to a new tab and pressed login. it took me to the google login page, i selected the mail id, but then it took me back to the login page. i tried again, it took me back to login again. 

so now there was this issue i had to resolve. GPT 5.2 kept telling me to recheck the environment variable URL and API key for supabase at the vercel project. i rechecked again and again. 

then it said that the issue could be that the url site at supabase might not be the correct address of the vercel homepage. checked, and it was correct. 

gpt 5.2 then hallucinated - in that after what it suggested was exhaustively checked, it suggested what i think a software engineer could immediately see to be random guesswork by the ai. it asked me to change the site url at supabase to some callback version of the vercel page. one that in hindsight feels stupid. 

the issue it turned out was that codex had another environment variable in the code that 5.2 didn't know or expect. and all i had to do was add that variable in the vercel settings. 

this took me probably more than 4 hours of focused work. in hindsight i think maybe i should've sticked to just codex. but no 5.2 did tell me once that what codex was proposing - bypassing rls policy and moving to server side (i have no idea what that means) was wrong. and so i had to ask codex not to do that. 

anyways this was one of the most difficult task i've accomplished with ai. and what it has managed to do is make me appreciate software engineers and all the people that work in the fields. it is complex. there were so many options and features just within these 3 sites i used - google cloud console, supabase and vercel. 

also i rarely did anything knowledgeable or value adding from myself. all i did was follow the llm's instructions and copy paste feed it the errors. 

which means that an agent could've done this whole task. an agent who used another llm as an auditor. interesting times we live in. the pace of improvement in ai technology is astounding. but whats even faster is the rate at which we get used to the technology. its actual magic but the magic rarely produces awe now.

the final product - 

![Yearly Distance](/assets/images/website.png)
