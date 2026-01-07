---
title: "TIL: manually getting YT music recap playlist through code and google takeout"
date: 2026-01-06
categories: til
---

i listen to a decent amount of music. in 2025 i listened to a lot of music in the first half because I had my ca final exams in may 2025 and i absolutely cannot self study without sountrack music. i listen to hans zimmer, ludwig, daft punk to name a few.

each year, i wait for the yt music recap feature because it gives me a playlist of the top 100 most listened songs of the year. a musical memory of sorts if i ever want to go down the nostalgia road in the future.

however this year - 2025 - i got the yt music recap slides but not the playlists. i waited, hoping the playlist would appear, but to no avail.

i remembered from earlier that there was this google website that lets you export all of your data - its called google takeout. i decided to use llms to manually make a playlist basis that data.

so i went to takeout and downloaded my data. i got 2 formats - json and html. json is the better language for machines and code but for some reason that i don't know why the json file only went back to april 2025 history. i asked gemini 3 pro to give me the code, copy pasted it to a text doc and saved it as .py, i opened powershell, ran the code, expected it to take some time but there it was - the top 100 songs - the code ran within less than a second. 

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

edit - since the code worked, it was natural to play along. althought the data attributes i have aren't a lot - i only have the song name and when it was played - there's still a lot i can do. 

first i also created a playlist without the soundtracks - fairly easy by asking the llm to remove songs by hans zimmer, ludwig and other instrumental artists. then the llm suggested a script to get -
1. top songs by each month - very interesting to see it. the brain is a victim of availability and recency bias and so actually looking at the data that defined you during that period of time is interesting and kind of cognitive dissonance like.
2. hourwise distribution of songs listened during. got a u-shaped distribution (peaks at the sides and zero at the middle. (basically im a night owl or atleast was during the study phase)
3. top 10 artists - top 4 matched with yt music recap slides, 5th didn't. most probable explanation is that the data i have doesn't take into account the amount of time i listened to a song while yt's code must have that as well. which is ironic about how takeout is still contrained by google's choice. maybe its for the better. i have no clue.

time to sleep.
