# commentary.vim


This is an adaptation of the vim-commentary <https://github.com/tpope/vim-commentary>
by Tim Pope <https://tpo.pe>.

commentary.vim comments stuff out.  Use `gcc` to comment out a line (takes a count),
`gc` to comment out the target of a motion (for example, `gcap` to
comment out a paragraph), `gc` in visual mode to comment out the selection,
and `gc` in operator pending mode to target a comment.  You can also use
it as a command, either with a range like `:7,17Commentary`, or as part of a
`:global` invocation like with `:g/TODO/Commentary`. That's it.

It uncomments, too.  The above maps actually toggle, and `gcgc`
uncomments a set of adjacent commented lines.

With this version, you can define g:space_after_commentstring to 1 or 0 to control whether
a space is inserted after the commentstring or not. It is the only difference.

## Installation

Install using your favorite package manager. Two examples.

> Vundle

    Plugin "zaikunzhang/vim-commentary"

> vim-plug

    Plug "zaikunzhang/vim-commentary"


## FAQ

> My favorite file type isn't supported!

Relax!  You just have to adjust `'commentstring'`:

    autocmd FileType apache setlocal commentstring=#\ %s


## Promotion

Like commentary.vim? Follow Tim Pope's repositories on
[GitHub](https://github.com/tpope/vim-commentary) and vote for it on
[vim.org](http://www.vim.org/scripts/script.php?script_id=3695).  And if
you're feeling especially charitable, follow [tpope](http://tpo.pe/) on
[Twitter](http://twitter.com/tpope) and
[GitHub](https://github.com/tpope).

## License

Distributed under the same terms as Vim itself.
See `:help license`.
