The support for Windows has been added but not tested extensively.
Windows users should consider the `original mcomix`_ if it just works.

=======
MComix3
=======

Fork from MComix gtk3 branch, switch to python3.

Only tested under Linux.

Required:
---------
- **Python3** 3.5 or later. `1`_
- **PyGObject** 3.24 or later `2`_, with **GTK+ 3 gir bindings** 3.22 or later.
- **Pillow** 5.2.0 or later. `3`_ (`Latest version`_ is always recommended)

Recommended:
------------
- **unrar**, **rar** or **libunrar** to extract RAR archives. `4`_
- **7z** `5`_ (**p7zip** `6`_ for POSIX system) to extract 7Z and LHA archives. Note that 7z might be able to extract RAR archives as well, but this might require additional software (for example, **p7zip-rar** on Debian-like systems), and it might fail to open certain RAR archives, especially newer ones.
- **lha** `7`_ to extract LHA archives.
- **mupdf** `8`_ for PDF support.
- **libflif_dec** or **libflif** `9`_ for FLIF support.

Run:
----
``python3 mcomix/mcomixstarter.py <diretory, archive or image>``

Run (Windows x86-64):
----
- Install **msys2** `10`_
- Within msys2, run ``pacman -S mingw-w64-x86_64-gtk3 mingw-w64-x86_64-python3 mingw-w64-x86_64-python3-gobject mingw64/mingw-w64-x86_64-python3-pillow``
- ``/mingw64/bin/python3 mcomix/mcomixstarter.py <diretory, archive or image>``

Install:
--------
**setup.py is not working**

``python3 installer.py --srcdir=mcomix --target=<somewhere>``

then:

``python3 <somewere>/mcomix/mcomixstarter.py <diretory, archive or image>``

.. _original mcomix: https://sourceforge.net/projects/mcomix/
.. _1: https://www.python.org/downloads/
.. _2: https://pygobject.readthedocs.io/
.. _3: https://pillow.readthedocs.io/
.. _Latest version: https://pypi.org/project/Pillow/
.. _4: https://www.rarlab.com/rar_add.htm
.. _5: https://www.7-zip.org/
.. _6: http://p7zip.sourceforge.net/
.. _7: https://fragglet.github.io/lhasa/
.. _8: https://mupdf.com/
.. _9: https://github.com/FLIF-hub/FLIF
.. _10: https://www.msys2.org/
