==========
dmenu-maim
==========

dmenu wrapper for maim (X11) or grim (Wayland), supporting saving to a file
and copying to the system clipboard, using the entire screen, a selection, or
the currently focused window.

Dependencies (X11): dmenu_, maim_ (and slop_), xdotool_, xclip_

Dependencies (Wayland): dmenu_, grim_, slurp_, wl-clipboard_

On Wayland, taking a screenshot of the selected window is currently only
supported on Sway_, because ``swaymsg`` is used to get the current window (as
in the example in |the grim README|_).

.. _dmenu: https://tools.suckless.org/dmenu/
.. _maim: https://github.com/naelstrof/maim
.. _slop: https://github.com/naelstrof/slop
.. _xdotool: https://www.semicomplete.com/projects/xdotool/
.. _xclip: https://github.com/astrand/xclip
.. _grim: https://wayland.emersion.fr/grim/
.. _slurp: https://wayland.emersion.fr/slurp/
.. _wl-clipboard: https://github.com/bugaevc/wl-clipboard

.. _Sway: https://swaywm.org/
.. |the grim README| replace:: the ``grim`` README
.. _the grim README:
   https://github.com/emersion/grim/blob/
   d570e13d6fa343507ebaafcc390142aa21cf591a/README.md

Arch Linux package
==================

Running ``makepkg --noextract`` should create an Arch Linux package. This
works because ``src/dmenu-maim`` is a symlink to the root of the repository.

License
=======

Copyright (c) 2020-21 Pratyush Venkatakrishnan

All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice,
   this list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
POSSIBILITY OF SUCH DAMAGE.

..
    vim: tw=77
