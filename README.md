# MagickaMod

This is a staging area for a personal patch that aims to fix critical game
breaking bugs in the original game while adding some quality of life
improvements.

It does not perform any of the following:

- No unlock for any paid content
- No bypass for game license check :exclamation:
- No bypass for game file integrity check

You are encouraged to buy a copy of the original game and apply this patch
(once it is available) through a script/installer that will update your game.

> [!NOTE]
> Long-term, the goal is to provide basic modding tools to add their own
> features as well, like an "RPG Mod" for persistent levelling and stats; or
> a "Custom Difficulty" mod that would allow players to adjust the amount of
> damage dealt/taken for a more comfortable experience.
>
> The priority is to make the game playable online, first.

## Features

The current work performed is as follows:

- Quality of Life
    - [x] Add borderless full-screen support
    - [ ] Retain player state (staff, weapon) when reloading from checkpoint
- Bug Fixes
    - [x] Fix crash due to repeated calls to web service
    - [ ] Fix various graphics-related crashes
    - [ ] Fix various crashes when loading into new scenes
        - Scenes are considered a "section" of a chapter
- Technical
    - [x] Always allow text input, even in single player (for in-game text commands?)
    - [x] Expand amount of memory available to Magicka up to ~4GB
    - [x] More verbose logging for debugging purposes
    - [x] Use UTC time when generating logs
    - [x] Update version string with mod version and config
    - [x] Pre-cache type data for faster lookups

## FAQ

### Where do I download it?

This mod is **not yet available**; it has been going through some private
testing to try to identify most of the immediate issues.

Unfortunately, some crashes are still happening either minutes into the game,
or seemingly never after hours of playing the game.

### In-Game Warning?

On launch, the game will represent you with a notice, stating the following:

> You are running a modified version of Magicka. Achievements, online
> leaderboards and VAC protected online games have been disabled. If this was
> not intentional, validate your game cache using the Steam client and restart
> the game. Otherwise, happy modding.

![Screenshot of the main menu, showing the "modified version" warning](.github/moddingAck.png)

This is actually included in the latest Steam release, so this notice is
retained to respect the original developer's wishes.

The version string in the bottom-left is also modified with an additional
mod version and configuration (Debug/Testing/Release) to help identify what
version of the game is running.

### Do I need to own the game to play this?

Yes, this is currently targeting the latest Steam release. (On release, this
will be replaced with a specific version once I bother to look it up.)

## Acknowledgements

This repository does not contain any files that are distributed with the game.

Third-party works and attributions are listed below.

### Paradox Interactive EULA and Modding

The [Paradox Interactive EULA][ParadoxEULA] documents their stance on modding plainly:

> We love when our community creates user-generated content, including mods, and
> we encourage you to do so! We hereby grant you the right to create, enjoy and
> make publicly available UGC, for non-commercial purposes. However, you are the
> creator of and responsible for the UGC that you create, and that UGC shall not
> contain any material which is unlawful, infringing, inappropriate, or violates
> any contracts or common sense. 

For the full text, see section 5 in the "Long Version" titled "User Generated
Content".

[ParadoxEULA]:https://legal.paradoxplaza.com/eula

### Magicka

Magicka was developed by Arrowhead Game Studios and published by Paradox
Interactive. Other developers have since contributed as well, such as
Pieces Interactive.
