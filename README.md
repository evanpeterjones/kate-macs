# Kate-macs
A config file containing a subset of the Emacs keybindings for the KDE Kate text editor.

# Getting Started
Open Kate and from the toolbar...
`settings > Configure Shortcuts... > Manage Schemes >> Import Scheme`
give it the `.shortcuts` file in this repo and you're off to the races!

# Contributing
This is incomplete.
I am familiar enough with Emacs to feel stunted by a lack of cursor control and multi-buffered views, but am by no means a power user and so have certainly missed many of the commands. So please feel free to make a pull request with whatever contributions if any of your favorite commands were unfortunately missed.

**It's _super easy_ to make changes! Load your '.shortcuts' file into Kate, make your changes in the same GUI used for import and then export the shortcuts file and send me a pull request**

# Current Issues
Some commands Kate does not support, such as C-l to cycle the view orientation around the cursor.
Larger packages like 'M-x replace-regexp' do not have support.
Certain compensations have been made, C-s & M-% both open a find-and-replace dialog, as an example.

# Working Commands
### kate_aliases = emacs-equivalent
```
beginning_of_document = M-<

beginning_of_line = C-a

delete_next_character = C-d

delete_word_right = M-d

edit_cut = C-w

edit_paste = C-w

edit_select_all = C-x, C-p

edit_undo = C-x, U

end_of_document = M->

end_of_line = C-e

file_close = C-x, C-c

file_open = C-x, C-f

file_save = C-x, C-s

go_goto_line = M-g, g

go_next_split_view = C-x, o

kate_mdi_toolview_kate_plugin_katesearch (find-and-replace) = -%;  C-s

move_cursor_right = C-f

move_cusor_left = C-b

move_line_down = C-n

move_line_up = C-p

scroll_page_down = C-v

to_matching_bracket = M-e

tools_cleanIndent = C-M-\\

tools_scripts_jumpIndentUp = M-a

view_split_horiz = C-X, 2

view_split_vert = C-X, 3

word_left = M-b

word_right = M-f
```

# Broken Commands
```
scroll_page_up = M-v		  : unknown why Kate finds this ambiguous?

(align view to cursor) = C-l 	  : no kate alias equivalent
```