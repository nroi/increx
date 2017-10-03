# increx

Elixir's IEx does not use readline, unfortunately. This makes navigating the history more difficult than it needs to be, especially
if you have gotten used to using readline with `history-search-forward` and `history-search-backward` (sometimes referred to
as incremental search, described in more detail [here](https://wiki.archlinux.org/index.php/Readline#History)).

increx does *not* add this functionality to IEx. Instead, it's a completely separate script with the sole functionality of
navigating through the history, with the added advantage of readline support. If you click enter, the current input will
simply be pasted into your clipboard.


## Installation & Configuration

Just copy both scripts into your `PATH`. If your Erlang history does not reside in `~/.cache/erlang-history/erlang-shell-log`,
update the path in the `increx` file.

If you haven't installed pyperclip, get it from pip:
`pip install  --user pyperclip`


## Usage

Move both scripts into your `PATH`, then run `ingrex`. Click the up-arrow key
<kbd>↑</kbd> to navigate through your history. Type the prefix of something you have previously typed in IEx and then
hit <kbd>↑</kbd> to make use of incremental search.
