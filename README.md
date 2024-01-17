# Welcome to spinner.nvim 👋

spinner.nvim is a single file, no-dependency plugin for Neovim. It's easy to add to your Lua project for better organization.

## Installation

To install spinner.nvim, simply move the `spinner.lua` file from this repository to a subdirectory in your Lua project directory. Once transferred, you can adjust the configuration table at the beginning of the file to suit your needs.

## Usage

Here's a basic example of how to use spinner.nvim:

```lua
local spinner = require('YOUR_PROJECT.spinner')

-- Display the spinner at the top right of the screen
spinner.show()

-- Or customize the position
spinner.show({
  relative = "editor",
  width = 1,
  height = 1,
  col = vim.o.columns - 1,
  row = vim.o.rows - 1,
})

-- Hide the spinner when it's done
spinner.hide()
```

## Configuration

You can customize the following values:

```lua
-- User configuration section
local config = {
  -- Show a notification when done (set to false to disable)
  show_notification = true,
  -- Name of the plugin
  plugin = "spinner.nvim",
  -- Spinner frames
  spinner_frames = {
    "⠋",
    "⠙",
    "⠹",
    "⠸",
    "⠼",
    "⠴",
    "⠦",
    "⠧",
    "⠇",
    "⠏",
  },
}
```

## Demo

[![Simple demo usage with gen.nvim](https://i.gyazo.com/7806f54956945800e0144edc4f0998da.gif)](https://gyazo.com/7806f54956945800e0144edc4f0998da)

## Support

If you find spinner.nvim helpful, please consider giving it a star! ⭐️
