# Spotify Chart Project

IS 4487 Business Analytics team project. Can we predict which tracks ranked 51–200 on Spotify’s Global Weekly chart will reach the Top 50 in the next four weeks? A weekly shortlist could help music editors decide which tracks to review for broader playlist placement.

## Data

Start with one row per track per chart week. Keep the week ending date, track ID, title, artist, rank, chart streams and weeks on chart. Remove duplicates by track ID and week. Use earlier charts to calculate rank and stream changes. Use the following four charts to label whether each track reached the Top 50.

- [Spotify Global Weekly chart](https://charts.spotify.com/charts/view/regional-global-weekly/latest)
- [Historical CSV covering 105 chart weeks](https://raw.githubusercontent.com/evadatadev/musiktrends-spotify/main/data/processed/hist_data_24-25.csv)
- [Spotify’s explanation of chart stream counts](https://support.spotify.com/us/artists/article/understanding-spotify-charts/)

## Analysis plan

1. Check that each week is complete and keep only features available at prediction time.
2. Compare logistic regression and random forest to a baseline that picks the five tracks closest to rank 50. Hold out newer weeks for testing and allow four weeks of follow-up for each example.
3. Report how many of each method’s five weekly picks actually reached the Top 50. Use the results to decide whether to recommend a trial with the editorial team.

## Deliverables

- Project proposal
- Documented Python notebook with two or three models
- Link to an 8–10 minute team presentation video
