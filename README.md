GenericMakefile
===============

A generic Makefile which automatically (re)compiles the program
consisting on the C/C++ sources in the current working directory
and/or its "src" subdirectory. It properly resolves the dependencies
between the files to avoid unnecessary recompilation.

The compilation flags are at the beginning of the Makefile. Feel free
to modify them directly or by exporting a suitable environmental
variables.

BUILD TARGETS
-------------

**DEFAULT**

A basic build with most warnings enables.

**RELEASE**

Optimization (`-O2`) enabled.

**DEBUG**

Optimization disabled and debugging symbols enabled.

**SANITIZER**

A build using the Clang compiler with one of its sanitizers enabled.
Defaults to the Address Sanitizer (ASan). The sanitizer to enable is
kept in the `SANITIZER` variable.

**CLEAN**

Removes the object files and the resulting executable.

**DISTCLEAN**

The same as `clean` plus removes the dependency file.

AUTHOR
------

Wojciech 'vifon' Siewierski < wojciech dot siewierski at gmail dot com >

COPYRIGHT
---------

Copyright (C) 2014  Wojciech Siewierski

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
