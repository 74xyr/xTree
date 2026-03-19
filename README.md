# TreeFeller

TreeFeller is a Paper plugin for Minecraft 1.21.x that makes tree cutting feel more natural and visually satisfying.

Instead of instantly removing the whole tree, the tree falls over with an animation, lands in the direction it actually falls, drops its loot near the impact point, and leaves behind a few scattered leaves for a nicer result.

The plugin is designed to feel immersive without turning tree cutting into an overpowered instant-break feature.

## Features

- Animated tree falling
- Trees fall away from the player
- Drops appear near the actual impact point
- Sounds and particles play on the correct side
- A few leaves are placed on the ground after impact
- Saplings, sticks and apples can drop naturally
- Sneaking lets players bypass the system and break blocks normally
- Axe-only support
- Improved detection to reduce false positives on player-built wooden structures
- Better separation of connected leaves between nearby trees
- Simple language/message system

## Supported server software

- Paper 1.21.x

Tested on:
- Paper 1.21.11

## Supported tree types

- Oak
- Birch
- Spruce
- Jungle
- Acacia
- Dark Oak
- Cherry
- Mangrove

## How it works

When a player breaks a log with an axe, TreeFeller checks whether the structure looks like a natural tree.

If it is detected as a valid tree:
- the tree is collected
- the blocks are replaced with animated displays
- the tree falls over
- sounds, particles and drops are spawned on the same side as the visual fall
- logs and natural loot are dropped near the landing point
- a few leaves are left on the ground for a more natural look

Sneaking while breaking a log bypasses the plugin and keeps normal block breaking behavior.

## Tree detection

TreeFeller includes extra checks to avoid treating random wooden builds as natural trees.

It also tries to separate leaves from nearby trees more carefully, so if two tree crowns touch, the plugin does not simply take every connected leaf block.

No automatic tree detection is perfect in every edge case, but the current system is built to be much safer than a simple "connected logs and leaves" approach.

## Installation

1. Download the latest release
2. Put the jar into your server's `plugins` folder
3. Start or restart the server

## Requirements

- Java 21
- Paper 1.21.x

https://i.ibb.co/KcFHNbHD/tree.gif
