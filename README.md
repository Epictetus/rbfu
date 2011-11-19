# rbfu

Because I've grown to dislike both RVM and rbenv -- too much magic. Here's
my attempt at a minimal solution.

### Installation

Simply clone the rbfu repository to `$HOME/.rbfu/`:

    git clone git://github.com/hmans/rbfu.git ~/.rbfu

Add the following line to your favorite startup script (eg. `.bash_profile`):

    eval "$(~/.rbfu/bin/rbfu-init)"

Don't forget to reload your shell environment or start a new shell session for the change to be picked up.

Finally, install your favorite Ruby versions through `rbfu-install` (this requires
[ruby-build](https://github.com/sstephenson/ruby-build) to be installed):

    rbfu-install 1.8.7-p352
    rbfu-install 1.9.2-p290
    rbfu-install 1.9.3-p0

### Usage

Switch Ruby versions using the `rbfu` command. For example:

    rbfu 1.8.7-p352

This will modify your current environment with all the paths and variables required for
the selected version of Ruby to be used.

### License

MIT License

Copyright (c) 2011 Hendrik Mans

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
