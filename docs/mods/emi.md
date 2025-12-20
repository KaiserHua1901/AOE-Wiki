# EMI ![EMI](img/EMI_icon.png){width=128; align=right}

EMI is a featureful and accessible item and recipe viewer.

## Want to learn about EMI?
**EMI**, or as we like to call it, your *Evolving Manufacturing Index*, is a browser that contains every single material, tool, block, resource, and fluid in this world. It gives you knowledge on how to craft everything and it will even show you how many resources it takes to craft something by pressing on the little tree icon next to the product lost of the recipe.

When in your inventory, on the right is your main browser. On your left will be your bookmarks.

#### Let's go over some actions.

- To find the recipe of an item, anywhere in a GUI, hover over it with your mouse and press the letter **R** on your keyboard. If you hover over the item *in* the recipe browser itself, you can simply **Left-Click** on it.
- To find the uses of an item, anywhere in a GUI, hover over it with your mouse and press the letter **U** on your keyboard. If you hover over the item *in* the recipe browser itself, you can simply **Right-Click** on it.
- To bookmark the item, hover over it in any GUI, and press the letter **A** on your keyboard.
- To bookmark a recipe, be in the window that shows a recipe, hover over the recipe (but *not* on a specific ingredient) and press the letter **A** on your keyboard.
- To un-bookmark an item/recipe, hover over the item/recipe in your bookmark section and press the letter **A**.
- To view a recipe tree that includes the total amount of resources to craft that item, press on the button that looks like the `T` shape from the hit game *Tetris*, usually to the right of the output slot in a recipe.
- To favorite a recipe and ensure your EMI views it as the default, press on the `❤` button usually to the right of the output slot in a recipe.
- To auto-fill a recipe into a workstation, open a valid workstation, open the recipe in your EMI, then press the `+` button, usually to the right of the output slot in a recipe.

## Searching

EMI offers special syntax for specific searches...

|   seach by:   |  syntax:  | matches items and blocks that...    |
| :-----------: | :-------: | ----------------------------------- |
|   ***mod***   | `@<foo>`  | ...have `<foo>` in their mod's name |
|   ***tag***   | `#<foo>`  | ...are tagged with `<foo>`          |
| ***tooltip*** | `$<foo>`  | ...have `<foo>` in their tooltip    |
| ***string***  | `"<foo>"` | ...have `<foo>` anywhere ^(1,^ ^2)^ |

...and search terms can be combined:

|   search phrase: | returns:                   |
| ---------------: | :------------------------- |
|    `<foo> <bar>` | `<foo>` *AND* `<bar>`      |
| `<foo> | <bar>`  | `<foo>` *OR* `<bar>` ^(3)^ |
|         `-<foo>` | *NOT* `<foo>`              |

Lastly, [regex](https://en.wikipedia.org/wiki/Regular_expression) search can be had with the form: `/<foo>/`.

!!! note "Notes on EMI's search syntax"
    1. `a b` matches `a b` *and* `b a`
    2. `"a b"` matches only `a b` (not `b a`)
    3. `a b | c` is the same as [`a` *AND* `b`] *OR* [`c`]

*Credit to *800020h* for collecting and making clear EMI's search abilities.*

<!-- Sub's outline notes
## Bookmarks

## Crafting Trees

TODO

- [ ] how to make and use them
- [ ] **synthetic bookmarks**
- [ ] tip about setting a, perhaps, more appealing background

## UI Options

TODO

- [ ] panel locations, and what they can show
- [ ] visual themes
-->

---
