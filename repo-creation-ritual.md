
The correct flow for a brand new repo:
gh repo create daily-checkin --public
gh repo clone lutwamahurbert/daily-checkin
cd daily-checkin
touch Readme.md
vim Readme.md
git add Readme.md          # ← the step you always forget
git commit -m "Initial commit"
git push -u origin main    # first push manually
After this first manual push, your us script will work fine on all future syncs since main will exist on the remote.
The memory trick: think of it as a 3-step ritual — add → commit → push. git commit never touches untracked/unstaged files directly.

