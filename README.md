# Project 2 - *Wordle 2*

Submitted by: **Daniella Michel**

**Wordle 2** is an iOS Swift-based clone of the popular word puzzle game, with extra knobs you can tweak. Players attempt to guess a hidden word; after each full-row guess, the app provides visual feedback using colored tiles:

- 🟩 **Green** — correct letter in the correct position  
- 🟨 **Yellow** — correct letter, wrong position  
- ⬛ **Gray** — letter not in the word

This version lets you choose the **word length (4–7 letters)**, the **number of guesses**, and a **theme** for the goal word. There’s also **Alien Wordle** mode where the goal word changes after each full-row guess. The interface uses UIKit with custom `UICollectionViewCell`s; the game auto-submits a row once it’s filled (no Enter key), and includes a top-left **Reset** button that clears the board without changing current settings.

Time spent: **15** hours in total

## Required Features

The following **required** functionality is completed:

- [x] User can change the number of letters per row (the length of the goal word)
- [x] User can change the numbers of rows on the board (how many guesses allowed)
- [x] User can select a new themed set to pull the goal word from
- [x] User can select "alien wordle", causing the goal word to change after each guess

The following **optional** features are implemented:

- [x] App displays a reset button on the top left to reset the game (but make no changes to the settings)

The following **additional** features are implemented:

- [ ] *(Add any extras you build later!)*

## Video Walkthrough

_Add a Loom (or GIF) walkthrough here._

**Example:**
- [Video Walkthrough](https://www.loom.com/share/bab1b3ea19224802912ab9e7368c87cf?sid=634c2269-114a-4d45-8e87-9da7317e8066)

## Notes

- Initially saw “no colors” because the **goal word length** didn’t match the selected letters-per-row; fixed by ensuring the generated goal always matches `numItemsPerRow`.
- Resolved settings lookups by using the settings dictionary keys in code where constants were unavailable.
- Minor Git issues (divergent histories, README conflict) were resolved via a merge.

## Technologies

- Swift, UIKit, `UICollectionView`
- Xcode 15+
- iOS 16+

## License

    Copyright [2025] [Daniella Michel]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
