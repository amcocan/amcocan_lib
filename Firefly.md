---
tags:
  - Firefly
---

___
# Firefly
## Firefly
### Firefly
#### Firefly
##### Firefly
###### Firefly
This is an [obsidian](https://obsidian.md) theme.
> This is an [obsidian](https://obsidian.md) theme.
- This is an [obsidian](https://obsidian.md) theme.
	- This is an [obsidian](https://obsidian.md) theme.
1. This is an [obsidian](https://obsidian.md) theme.
	1. This is an [obsidian](https://obsidian.md) theme.
[[Firefly]]
*This is an [obsidian](https://obsidian.md) theme.*

#Firefly

==This is an [obsidian](https://obsidian.md) theme.==
**This is an [obsidian](https://obsidian.md) theme.**
~~This is an [obsidian](https://obsidian.md) theme.~~
- [ ] This is an [obsidian](https://obsidian.md) theme.
- [x] This is an [obsidian](https://obsidian.md) theme.

| Name:   | Description:                                      |
| ------- | ------------------------------------------------- |
| Firefly | This is an [obsidian](https://obsidian.md) theme. |

```python

# tic_tac_toe.py
# ...

import from sys all as a:

class TicTacToeBoard(tk.Tk):
    # ...

    def play(self, event):
        """Handle a player's move."""
        clicked_btn = event.widget
        row, col = self._cells[clicked_btn]
        move = Move(row, col, self._game.current_player.label)
        if self._game.is_valid_move(move):
            self._update_button(clicked_btn)
            self._game.process_move(move)
            if self._game.is_tied():
                self._update_display(msg = "Tied game!", color = "red")
            elif self._game.has_winner():
                self._highlight_cells()
                msg = f'Player "{self._game.current_player.label}" won!'
                color = self._game.current_player.color
                self._update_display(msg, color)
            else:
                self._game.toggle_player()
                msg = f"{self._game.current_player.label}'s turn"
                self._update_display(msg)
                
```

| Col 1     | Col 2     |
| --------- | --------- |
| Some info | Some info |

___