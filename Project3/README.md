# My Movie Recommendation System

For this CodSoft task, I made a small movie finder called Frame. It helps me choose what to watch by matching movies to the genres, moods, and runtime I select. I designed it as a clean discovery dashboard, with a preference panel and ranked movie cards that explain why each title appeared.

## Try it out

1. Open `index.html` in a modern web browser.
2. Choose one or more genres and moods, then pick a runtime.
3. Select **Find my next film** to see the recommendations.
4. Use **Mark seen** to keep track of titles, or **Hide seen** to remove them from the list.

The page starts with science fiction and imaginative themes selected. You can change those choices at any time. The movie list and watched marks are kept in the page while it is open; the app does not use an account or send data to a server.

## How the recommendations work

I used a simple **content-based filtering** approach. Each movie has genre and mood tags. The app compares those tags with the preferences selected by the user and gives each matching genre 3 points and each matching mood 2 points. It sorts the matching movies by score, then applies the runtime and seen filters. Each card shows the matching preferences so the recommendation is easy to understand.

This is a small demonstration, so its suggestions are limited to the movie collection included in the code. It does not learn from other users or use collaborative filtering.

## What I learned

This project helped me understand how item features can be used to rank recommendations. I also practiced building preference controls, sorting results by a score, and showing a clear reason for each match.

## Project files

- `index.html` contains the dashboard, movie collection, and recommendation logic.
- `README.md` explains how to run the app and how its scoring works.
- `Project_Report.pdf` is a short report for my project submission.
