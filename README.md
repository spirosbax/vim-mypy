# vim-mypy

Vim plugin for executing Python's optional static type checker [MyPy](http://mypy-lang.org/).  
This is a fork of the [original](https://github.com/Integralist/vim-mypy) plugin by [Integralist](https://github.com/Integralist) made for maintenance purposes.

## Example

```py
def example(n: int) -> str:
    print(type(n))
    return 'hello'

example("a")  # << incorrect, we've passed a String and not an Integer 
```

To trigger the plugin, execute either `:Mypy` or the mapping `<Leader>mp`

## Install

### [Pathogen](https://github.com/tpope/vim-pathogen)

```bash
git clone https://github.com/spirosbax/vim-mypy ~/.vim/bundle/vim-mypy
```

### [Vundle](https://github.com/gmarik/vundle)

```
Plugin 'spirosbax/vim-mypy'
```

### [Vim-Plug](https://github.com/junegunn/vim-plug)

```
Plug 'spirosbax/vim-mypy'
```

## Alternatives

It seems both [Syntastic](https://github.com/vim-syntastic/syntastic) and [Neomake](https://github.com/neomake/neomake) include support for MyPy.
