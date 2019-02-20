# Vim Crutches

Vim crutches is a collection of Snippets that aim to balance speed with the need
for some repetition to commit knowledge to memory.

These are minimal and intended to replace boilerplate _only_.

This plugin requires [UltiSnips](https://github.com/SirVer/ultisnips).

## Installation

Example when using [vim-plug](https://github.com/junegunn/vim-plug), adapt to
your plugin manager of choice.

```vim
Plug 'miguelverissimo/vim-crutches'
```

**Optional:** [UltiSnips](https://github.com/SirVer/ultisnips) triggers
configuration:

```vim
let g:UltiSnipsExpandTrigger="<C-l>"
let g:UltiSnipsJumpForwardTrigger="<C-]>"
let g:UltiSnipsJumpBackwardTrigger="<C-[>"
```

## Usage

Some of the snippets will infer defaults from the file name. For example, if you are editing a file called `HomePage.js`, and in _insert_ mode you type:

```vim
rfc<C-l>
```

Will be expanded to
```javascript
const HomePage = (props) => (
  <div>

  </div>
)

export default HomePage;
```

I'm trying to keep the snippets in a mnemonic style of shortcut, where the first
char will be for the technology, and the remainder for the actual component.

All snippets are in [`UltiSnips/javascript.snippets`](UltiSnips/javascript.snippets).

## Snippets List

### ES2015+
| Trigger | Produces |
| ------: | -------- |
| `c` | const |
| `l` | let |
| `i` | import |
| `e` | export |
| `r` | return |
| `map` | method with function |
| `filter` | method with function |
| `forEach` | method with function |
| `reduce` | method with function |
| `=>` | arrow function |
| `c=>` | const function |
| `cex` | const function with export |
| `forof` | for .. of .. |
| `class` | class |
| `cl` | console.log |


### React

| Trigger | Produces |
| ------: | -------- |
| `rcc`   | React **Class** Component |
| `rfc`   | React **Functional** Component |

## Credits

Most of the snippets were ripped off, or heavily inspired by [Emmanuel
Pillande's](https://github.com/epilande) [Vim React Snippets](https://github.com/epilande/vim-react-snippets) and [Vim ES2015 Snippets](https://github.com/epilande/vim-es2015-snippets)

## License
[MIT/X11](https://en.wikipedia.org/wiki/MIT_License)
