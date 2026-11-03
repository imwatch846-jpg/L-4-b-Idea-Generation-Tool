# L-4-b Idea Generation Tool

A team tool for the L-4-b Idea Generation assignment: brainstorm artifacts, musts and wants, merge duplicates, group ideas into categories, multi-vote, and summarize.

## Files
- `index.html` : the whole website (no build step)
- `README.md` : this file

## Publish on GitHub Pages
1. Create a new GitHub repository.
2. Upload `index.html` (and this README).
3. Settings → Pages → "Deploy from a branch" → branch `main`, folder `/ (root)` → Save.
4. Your site appears at `https://<username>.github.io/<repo>/` after a minute or two.

## Optional: live sharing for all 5 members (free)
Without this step the site works, but each phone keeps its own separate data.

1. Go to https://console.firebase.google.com and create a project (the free Spark plan needs no payment method).
2. Build → Realtime Database → Create database.
3. Open the **Rules** tab and paste the rules below, then Publish. (Test mode expires after about 30 days; these rules do not.)

```json
{
  "rules": {
    ".read": true,
    ".write": true
  }
}
```

4. Copy the database URL from the **Data** tab (looks like `https://yourproject-default-rtdb.firebaseio.com`).
5. In `index.html`, find `const DB_URL="";` near the top of the script and paste the URL between the quotes. Optionally change `ROOM` to your team's name.
6. Commit the change. Everyone who opens the Pages link is now on the same live data.

Anyone who has the database URL can read and edit the data, so do not put anything private in it.

## How the team uses it
1. Everyone opens the link and picks their member symbol (1 to 5).
2. **Brainstorm (hidden):** add ideas. You only see your own ideas. Tap “I'm finished” when done; ideas are revealed to everyone once all five have finished (or someone taps “Reveal now”). For wants, use the Random Stimulation words when ideas dry up.
3. **Merge & group:** merge duplicates (the tool suggests likely matches), choose the best wording, and assign categories.
4. **Multi-vote:** each member has about 1/3 of the list as votes. Then keep the top ideas.
5. **Summary:** check the checklist, copy the final picks onto the official sheet **by hand**, and download the full record for your notebook.

## Targets from the assignment
| List | Brainstorm | Keep after multi-voting |
|---|---|---|
| Artifacts | at least 20 | 6 to 10 |
| Musts | at least 10 | at least 3 |
| Wants | at least 10 | 3 or 4 (with weights) |
