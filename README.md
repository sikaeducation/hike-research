# Hike Research

You've just been on the worst hike of your life and decide you need to explore
your options for a better hike next time. Look at a few different hiking boot
options and choose the right one for your next trip.

## Instructions

1. Clone this repository to your computer and navigate to it using your terminal
2. Run `./start` in your terminal to begin the game. You'll be sent to a random
   commit in the repository to learn about an item that can help you have better
   hikes.
3. Keep running `./next` in the terminal to see more items. After you've seen 5
   of them, you'll be automatically sent back to the `main` branch.
4. Use Git's `reflog` feature to navigate to the indicated commit.
5. Run `./finish` to in your terminal to check your work!

If you make a mistake, run `./start` to start over.

## Tips

### Navigating the Git Reflog

While a Git repo's `log` shows the commits that came before it, the `reflog`
shows all of the places you've previously been. These commands will be useful
for this game:

- `git reflog` - See a list of commits you've seen, with the most recent commit
  first
- `git checkout ref-goes-here` - Switch to a different commit. In this case, a
  _ref_ can either be:
  - At least the first 4 characters of the commit's _hash_, such as
    `git checkout a5d7`. This will switch to the commit that has a hash starting
    with `a5d7`.
  - A _relative ref_ based on your history, such as `git checkout HEAD@{2}`.
    This will switch to the last commit you looked at, regardless of what branch
    it's on.

[Game 3](https://github.com/sikaeducation/hike-plan)
