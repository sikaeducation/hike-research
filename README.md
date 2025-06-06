# Hike Research

You've just been on the worst hike of your life and decide you need to explore
your options for a better hike next time. You decide to look at a few different
hiking boot options to choose the right ones for your next trip.

## Instructions

1. Clone this repository to your computer and navigate to it using your
   terminal.
2. Run `./new-game` in your terminal to begin the game. You'll be sent to a
   random commit in the repository to learn about a different pair of boots.
3. Follow the on-screen instructions to finish the game!

If you make a mistake, run `./new-game` to start over.

## Tips

While `git log` shows the preceding commits in the current branch, `git reflog`
shows all of the commits you've previously visited. One way to think of this is
that everyone will see the same `git log` for a branch, but everyone's
`git reflog` will be different. The log is the code's history; the reflog is the
user's history.

These commands will be useful for this game:

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

## Relevance

The reflog is useful for lots of situations:

- If you make a mistake with a destructive command like `git reset --hard`, the
  reflog can help you find a previous version to restore.
- When you're jumping between many different branches, the reflog acts like a
  map of all the places you've been so you can find your way back easier.
- Even the first 4 characters of a commit hash can be hard to remember; using
  relative commands like `git checkout HEAD@{2}` is almost always easier.
- The reflog remembers commits that aren't even part of a branch anymore.

[Game 3](https://github.com/sikaeducation/hike-plan)
