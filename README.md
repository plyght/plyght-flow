# Flow Control: a programmer's text editor

This is my Zig text editor. It is very much a work-in-progress, but far enough along that I am daily driving it.

features:
- fast TUI interface. no user interaction should take longer than one frame (6ms) (even debug builds)
- tree sitter based syntax highlighting
- multi cursor editing support
- first class mouse support (yes, even with a scrollbar that actually works properly!)
- vscode compatible keybindings (thanks to kitty keyboard protocol)
- vim compatible keybindings (at least the basics, more to come)
- good unicode support
- hybrid rope/piece-table buffer for fast loading, saving and editing with hundreds of cursors
- theme support (compatible with vscode themes via the flow-themes project)
- infinite undo/redo (at least until you run out of ram)
- stuff I've forgotten to mention...

features in progress:
- LSP support for linting and navigating
- find in files
- multi tty support (shared editor sessions across multiple ttys)
- command palette
- completion UI
- persistent undo/redo

features planned:
- multi host editing
- multi user editing
