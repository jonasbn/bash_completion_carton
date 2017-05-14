# Carton Bash Completion

Incredibly basic `bash` completion for Perl's [carton](https://github.com/perl-carton/carton).

## Usage

```
$ carton <tab>
bundle exec     help     install
```

See [carton](https://github.com/perl-carton/carton) for more information on the different commands available to carton, can also be retrieved via `carton help`.

`install` offers additional completions.

```
$ carton install <tab>
--cached      --deployment
```

## Installation

```bash
$ curl https://raw.githubusercontent.com/jonasbn/completion-carton/master/carton > carton
```

Where your completions are located might vary:

Based on [an introduction](https://debian-administration.org/article/316/An_introduction_to_bash_completion_part_1) to `bash` completions on Debian.

```bash
$ sudo cp carton /etc/bash_completion.d/
```

This is not a part of [the completions](https://github.com/Homebrew/homebrew-completions) available under `brew` on OSX. But you can copy the `carton` file to the same directory:

```bash
$ cp carton /usr/local/etc/bash_completion.d/
```

And to activate right away:

```bash
$ . /usr/local/etc/bash_completion.d/carton
```

## Motivation

I have not used `bash` tab completions before, but I fell over [this blog post](http://davidalger.com/development/bash-completion-on-os-x-with-brew/). So this is my first *shot* at creating a `bash` completion for a command I use a lot.

## See Also

A more elaborate piece of documentation on `bash` completions is available from **The Linux Documentation Project** in the [Advanced Bash-Scripting Guide](http://tldp.org/LDP/abs/html/tabexpansion.html).

From the [GNU Documentation](https://www.gnu.org/software/bash/manual/html_node/Programmable-Completion.html).

Good two-part article, "An Introduction to Bash Completion": [Part 1](https://debian-administration.org/article/316/An_introduction_to_bash_completion_part_1) and [Part 2](https://debian-administration.org/article/317/An_introduction_to_bash_completion_part_2).

Please note that this experimental implementation has only been tested with `bash` version 3.

## License

This is made available under the MIT license, see separate license file.

## Copyright 

:copyright: jonasbn 2016-2017
