# Contribution [#]: [Issue Title]

**Contribution Number:** [1 / 2 / 3]  
**Student:** [Ella]  
**Issue:** [https://github.com/wesnoth/wesnoth/issues/1559]  
**Status:** [Phase I] [Complete]

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

1. Build from the command line with CMake:
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

**Understand:** Add a volume attribute to the game

**Match:** There are existing attributes under the music tag in which I can see how.

**Plan:** 
1. Modify the sound file.
2. Add the volume attribute to controle the sound level.
3. Run the build

**Implement:** [Link to your branch/commits as you work]

**Review:** 

**Evaluate:** See if creators can modify the song volumes by running the game and running it on my own.

---

## Testing Strategy

### Unit Tests

- [ ] Test case 1: [Description]
- [ ] Test case 2: [Description]
- [ ] Test case 3: [Description]

### Integration Tests

- [ ] Integration scenario 1
- [ ] Integration scenario 2

### Manual Testing

[What you tested manually and results]

---

## Implementation Notes

### Week [X] Progress

[What you built this week, challenges faced, decisions made]

### Week [Y] Progress

[Continue documenting as you work]

### Code Changes

- **Files modified:** [List]
- **Key commits:** [Links to important commits]
- **Approach decisions:** [Why you chose certain approaches]

---

## Pull Request

**PR Link:** [GitHub PR URL when submitted]

**PR Description:** [Draft or final PR description - much of the content above can be adapted]

**Maintainer Feedback:**
- [Date]: [Summary of feedback received]
- [Date]: [How you addressed it]

**Status:** [Awaiting review / Iterating / Approved / Merged]

---

## Learnings & Reflections

### Technical Skills Gained

[What you learned technically]

### Challenges Overcome

[What was hard and how you solved it]

### What I'd Do Differently Next Time

[Reflection on your process]

---

## Resources Used

- [Link to helpful documentation]
- [Tutorial or Stack Overflow post that helped]
- [GitHub issues or discussions that helped]
