# Contribution [#1]: [Adding the feature to adjust volume to music tracks in a video game]

**Contribution Number:** [1]  
**Student:** [Ella]  
**Issue:** [https://github.com/wesnoth/wesnoth/issues/1559]  
**Status:** [Phase IV] [Complete]

---

## Why I Chose This Issue
I enjoy working with video games, and I also have an interest in volume/audio. This issue was under an open-source video game, and it was also labeled as an audio issue. Moreover, it was also labeled a "Good First Issue." They have labels like that for anyone new to contributing, and I believed it to be an active community with a Discord too.

I hope to learn how to contribute to open-source games.

---

## Understanding the Issue

### Problem Description

I'm supposed to create a feature that allows for songs to be specified at different level. 

### Expected Behavior

The feature should work the same way as the volume tag does in the game.

### Current Behavior

Developers of campaign creators aren't able to add a volume attribute.

### Affected Components

The src/sound/ part of the codebase is involved.
---

## Reproduction Process

### Environment Setup

I faced a challenge in which I had trouble running because the buld was missing a .nib file which allowed the game to be called and run, but I made that into another github issue.

### Steps to Reproduce

1. Build from the command line with CMake.
2. Run the resulting binary from Terminal:
3. The process was hanging, so I added a MacOS launcher for the build to make it run.

### Reproduction Evidence

- **Branch showing reproduction:** https://github.com/iwasella/wesnoth/tree/feature/1559-music-volume-attribute
- **My findings:** There isn't a MacOS launcher for the build. 

---

## Solution Approach

### Analysis

There isn't really an issue, but I hope to add a new attribute.

### Proposed Solution

I plan on going into the src/sound of the repo and looking into how they create attributes specifically for the music tag in the game. Then, I pla on adding the volume attribute.

### Implementation Plan

**Understand:** Adding the volume attribute to the music track involves understanding that the Wesnoth Markup Language.

**Match:** There are existing attributes under the music tag in which I can see how to better implement

**Plan:** 
1. Modify the files that work in relation to the sound.
2. Add the volume attribute to controle the sound level.
3. Run the build everytime I make a change to see how it works.

**Implement:** [Branch which adds volume attribute](https://github.com/iwasella/wesnoth/tree/feature/1559-music-volume-attribute)

**Review:** 

**Evaluate:** See if creators can modify the song volumes by running the game and running it on my own.

---

## Testing Strategy

### Unit Tests

- [X] Test case 1: Worked on a single track which happened to be on the titlescreen and initialized the volume attribute to see that it really does scale down.
- [X] Test case 2: Making sure that the volume is being scaled in relation with the preference music slider


### Manual Testing

- Playing the test track with the game titlescreen and actively using the music preference slider

---

## Implementation Notes

### Week [2] Progress

I worked on reading the docs on the Wesnoth website, and I built up adding the volume attribute to the files. My biggest challenge figuring out which files I was suppoed to look at in the codebase. I decided to look into src/sound. I made a PR and got feedback.

### Week [3] Progress

With help from others, I reworked on my branch, making sure that nothing is overwritten in regards to the preference slider.

### Code Changes

- **Files modified:** Mainly sound.cpp and sound_music_track.cpp
- **Key commits:** [When I first added the volum attribute](https://github.com/wesnoth/wesnoth/commit/fd670b927f4291e51f2724bba093619276e20a37) <br>
[Fixing bugs with the volume attribute](https://github.com/wesnoth/wesnoth/commit/a1c81c52935c6dcb3f540a4d10eed973db1bba09)
- **Approach decisions:** I worked a lot on the titlescreen because it was easier for me to load that scenario.

---

## Pull Request

**PR Link:** https://github.com/wesnoth/wesnoth/pull/11291

**PR Description:** [I added the Volume Attribute]

**Maintainer Feedback:**
- [June 15th]: Track specific volume is overwritten using slider. Check the '''set_music_volume'''.
- [June 15th]: Worked on making sure the slider works in relation with the track volume.
- [Month of July]: Rework on clamping the audio.

**Status:** [Awaiting review]

---

## Learnings & Reflections

### Technical Skills Gained

I got more experience with learning a new codebase and how audio in c++ can be handled.

### Challenges Overcome

I was not used to interacting with a new community to open-source, but I joined the Discord Server and also maintain active comms in regards to PR feedback.

### What I'd Do Differently Next Time

I'd fork and run a build to see where the bug is before I dive into a PR

