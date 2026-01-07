---
title: "TIL: manually getting YT music recap playlist through code and google takeout"
date: 2026-01-06
categories: til
---

i listen to a decent amount of music. 2025 i listened to a lot of music in the first half because I had my ca final exams in may 2025 and i absolutely cannot self study without sountrack music.

i wait for the yt music recap feature because it gives me a playlist of the top 100 most listened songs of the year. a musical memory of sorts if i ever want to go down the nostalgia road in the future.

however this year - 2025 - i got the yt music recap slides but not the playlists. i waited but to no avail.

i remembered from earlier that there was this google website that lets you export all of your data - its called google takeout. i decided to use llms to manually make a playlist basis that data.

i got 2 formats - json and html. json is the better language for machines and code but for some reason that i don't know why the json file only went back to april 2025 history. i asked gemini 3 pro to give me the code, copy pasted it to a text doc and saved it as .py, i opened powershell, ran the code, expected it to take some time but there it was - the top 100 songs - the code ran within less than a second. 

it felt truly magical. awe like. 

but this wasn't the whole truth (didn't intend to but i realised i just wrote down the name of the currently in good demand health brand). 

so i asked gemini to write me a code for the html file because it had the full 2025 year data. it used beautifulsoup library in the first try but the code took >5 minutes. so then i stopped it and told it and it changed the code to regex. 

the regex code failed several times but all i had to do was paste the error/output back to gemini. it iterated. and there i had it finally. my yt music recap playlist of 2025. 

the top 10 songs extract from the output - 
--- Top 100 Songs (2025-01-01 to 2025-12-31) ---
Found 20434 valid plays in this date range.
1. Open Hearts - The Weeknd - Topic (60 plays)
2. FOILS - Ludwig Göransson - Topic (46 plays)
3. Fission - Ludwig Göransson - Topic (45 plays)
4. Groves - Ludwig Göransson - Topic (43 plays)
5. Kiss the Ring - Hans Zimmer - Topic (43 plays)
6. 747 - Ludwig Göransson - Topic (43 plays)
7. Meeting Kitty - Ludwig Göransson - Topic (40 plays)
8. Lose My Mind (feat. Doja Cat) (From F1® The Movie) - Don Toliver - Topic (39 plays)
9. TRUCKS IN PLACE - Ludwig Göransson - Topic (39 plays)
10. THE ALGORITHM - Ludwig Göransson - Topic (39 plays)

whats amazing is how this got me into flow state. i feel contempt. not pleasure or happiness of sort but so relieved and contempt and motivated and awelike. 

so much so that i decided it was time to add a TIL section to my personal website. the brain is weird. 
