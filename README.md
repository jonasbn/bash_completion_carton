# Carton Bash Completion

Incredibly basic `bash` completion for Perl's [carton](https://github.com/perl-carton/carton).

I have not used `bash` tab completions before, but I fell over [this blog post](http://davidalger.com/development/bash-completion-on-os-x-with-brew/). So this is my first *shot* at creating a `bash` completion for a command I use a lot.

A more elaborate piece of documentation on `bash` is also available from **The Linux Documentation Project** in the [Advanced Bash-Scripting Guide](http://tldp.org/LDP/abs/html/tabexpansion.html). Another insightful read is the [project description](http://freecode.com/projects/bashcompletion).

## Usage

```
$ carton <tab>
bundle exec     help     install
```

See [carton](https://github.com/perl-carton/carton) for more information on the different commands available to carton, can also be retrieved via `carton help`.

`install` offers addional completions.

```
$ carton install <tab>
--cached      --deployment
```

## Installation

```bash
$ curl https://raw.githubusercontent.com/jonasbn/completion-carton/master/ > carton
```

Where your completions are located might vary:

Based on [an introduction](https://debian-administration.org/article/316/An_introduction_to_bash_completion_part_1) to `bash` completions on Debian.

```bash
$ sudo cp carton /etc/bash_completion.d
```

This is not a part of [the completions](https://github.com/Homebrew/homebrew-completions) available under `brew` on OSX. But you can copy the `carton` file to the same directory:

```bash
$ cp carton /usr/local/etc/bash_completion.d
```

## License

This is made available under the MIT license, see separate license file.

## Copyright 

:copyright: jonasbn 2016
