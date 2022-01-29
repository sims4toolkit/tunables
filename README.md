# Sims 4 Toolkit - Tunables (@s4tk/tunables)

## Overview

This project contains utility functions for creating tunable nodes.

**PLEASE NOTE**: Proper documentation for this package will be provided when the Sims 4 Toolkit website has been completed. Please be patient, because this will take a little while to finish. For now, reference this README's Documentation section for a basic introduction, and feel free to browse the [source code on GitHub](https://github.com/sims4toolkit/tunables.git) as needed. Every class, type, and function has thorough documentation available in the comments, and this should be enough to understand how the library works for now.

## Installation

Install the package as a dependency from npm with the following command:

```sh
npm i @s4tk/tunables
```

## Disclaimers

Sims 4 Toolkit (S4TK) is a collection of creator-made modding tools for [The Sims 4](https://www.ea.com/games/the-sims). "The Sims" is a registered trademark of [Electronic Arts, Inc](https://www.ea.com/). (EA). Sims 4 Toolkit is not affiliated with or endorsed by EA.

All S4TK software is currently considered to be in its pre-release stage. Use at your own risk, knowing that breaking changes are likely to happen.

## Documentation (WIP)

**PLEASE NOTE**: This documentation is by no means complete. The Sims 4 Toolkit website is being worked on, so please be patient. If you need additional documentation, feel free to check out the [source code on GitHub](https://github.com/sims4toolkit/tunables.git) for now.

### Importing

Import the utility functions from `@s4tk/tunables`

```ts
import { T, U, ... } from "@s4tk/tunables"; // ESM
const { T, U, ... } = require("@s4tk/tunables"); // CJS
```

### Functions

Functions for tunable nodes include `T`, `E`, `L`, `U`, and `V`.

You can also create instance nodes with `I`, and modules with `M`. Add classes to modules with `C`.

Add comments with `Comment`.

To automatically hash a string, add it to a string table, and turn it into a node (like `<T>0x00000000<!--String--></T>`), use `LocString`.

Use `getLocStringFn` as shorthand for `LocString`, so you don't have to pass the string table every time it's called, like so:
```ts
const stbl = StringTableResource.create(); // from @s4tk/models
const LocString = getLocStringFn(stbl);
```
