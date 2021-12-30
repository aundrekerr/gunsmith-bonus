# Gunsmith Bonus

This is a collection of all the little bonus data that you see on d2gunsmith.com. Keeping it here should let others see what's outdated, get it updated, and maybe let other apps use this data. For now, the formatting is staying simple enough to benefit anyone who chooses to use this repo. If I ever find a solution to store more rich data (that works universally, not a Gunsmith-specific solution) then it could see an update.

## Basic Format

```
// <name>
<hash>: <string>
```

It's nothing crazy. Just a comment, key, and value. For ease of use, head over to the [Destiny Sets API Explorer](https://data.destinysets.com) and find the hash of the thing that you're adding/updating. Remember that some things have multiple instances that function differently. For example, there are two Rampage traits. One is used on your average weapon that can roll the trait, and the other is exclusively for The Huckleberry Exotic SMG (it still has pre-Shadowkeep damage properties). 

**Don't forget to leave the comment with the name of the entry and a trailing comma.**

- `name` - Literally just the name of whatever it is. Two slashes before it to turn it into a comment.
- `hash` - The item's hash under the correct table (ex. Kill Clip is `1015611457` under "InventoryItem" [the one we want] but is also `2750005406` under "SandboxPerk").
- `string` - A basic text string. Try to avoid massive blocks of text and condense information as much as possible. Use bullets (`•`), new lines (`\n`), and tabs (`\t`) when suitable.

### A real example

```
// High-Impact Reserves
2213355989: "Gradual damage increase starting at 50% of magazine left.\n• \tIn PvE, 12.1% to 25.6%.\n• \tIn PvP, 3% to 6%.",
```
