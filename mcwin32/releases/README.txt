
Native GNU Midnight Commander for Win32
--------------------------------------------

Windows XP+/32 bit native port of GNU Midnight Commander, based on
the current 4.8.x development stream.

        Version         Build Notes

        4.8.33          233

                                - internal tools

                                        o mcupdater
                                            - Ed25519 support (#129) libappupdater-1.0.3
                                            - utilize GitHub for updater (#127)
                                        o mchelp locale (#126)
                                        o mcstart enhancements (#124)

                                - upgrades/bug-fixes

                                        o handle resource leak (#128)

        4.8.33          232

                                - internal tools

                                        o mandoc / mchelp integration (#116)
                                        o mcstart, file-extension utility (#124)
                                        o mc-wrapper's (#69)

                                - upgrades/bug-fixes

                                        o documentation enhancements
                                        o MSTerminal maximize disabled (#122)
                                        o obey NODRIVES group policy (#121)
                                        o getmntinfo, networked/mapped drive (#120)
                                        o script enhancements, MC_XDG_OPEN as "start" (#119)
                                        o non-ascii group name handling (#118)
                                        o stat/seek64 (#35) and (#89)
                                        o unzip vfs (#88)
                                        o ESC timeout, -1 enables an infinite wait (#36)

        4.8.33          231 (mc merge 4.8.33)

                                - internal tools front-ends, externalized (#78)

                                        o mcedit
                                        o mcdiff and mcbsddiff (diff backend)
                                        o mcview

                                - upgrades/bugfixes

                                        o vio: wide-character handling (#115)
                                        o wputenv() cross tool-chain usage (#113)
                                        o pcre2 10.45 (#106)
                                        o appupdater (#102)
                                        o glib 2.54.3 (#102)
                                        o zlib-1.3.1 (#102)
                                        o mbedtls-3.6.2 (#100)
                                        o improved UNC and extended prefix support, plus stat optimisations (#98)
                                        o libssh2-1.11.1 (#95)
                                        o enhanced utf8 support, directory plus username; non-ascii user name support (#97)
                                        o EXDEV, cross-device detection rename failure; allowing alt move logic (#85)
                                        o x64 installer path (#79)

        4.8.31          230 (mc merge 4.8.31)

                                 - mbedtls 3.5.2 (#67)
                                 - AltGr detection (#71, #52)
                                 - mcdiff integration (#74)
                                 - cd/cdpath (#72)

        4.8.30          229 (mc merge 4.8.30)

                                 - pcre2 10.42
                                 - mbedtls 3.4.1
                                 - enca 1.19
                                 - file 5.45
                                 - zlib 1.3

        4.8.29          228 (mc merge 4.8.29)

                                 - libssh2 1.11.0
                                 - mbedtls 3.3.0
                                 - zlib 1.2.11

        4.8.28          227 (mc merge, 4.8.27)

        4.8.27          226 (#21 - FISH enabled)

                                FISH requires either an external SSH and/or RSH client, possible solutions include:

                                o Windows portable OpenSSH [[ https://github.com/PowerShell/openssh-portable ]].
                                o WinXSH [[ https://github.com/adamyg/winxsh ]].

        4.8.27          225 (enhancements #16 and #17).
        4.8.27          224 (mc merge, libaspell - beta) See [https://github.com/adamyg/aspell-win32] for distributions.

        4.8.24          223 (bug fixes - unable to load skins)
        4.8.24          222 (UTF8 exec/shell support, libmagic upgrade)
        4.8.24          221 (bug fixes - whitespace handling, mbedtls and libssh2 upgrades)
        4.8.24          220 (UTF8/widechar file support)

        4.8.24          217 (enhancements / bug fixes / InnoSetup 5.x - beta3)
        4.8.24          216 (bug fixes - beta2)
        4.8.24          215 (beta)

        4.8.21          214 (bug fixes)
        4.8.21          213 (windows 10 console)
        4.8.21          209 (windows 10 console, beta)

        4.8.19          204 (configuration updates), 201 (sftp/ssh)

        4.8.14          189 (beta)

        4.8.13          188, 187 (beta)

        4.8.12          186
        4.8.11          183
        4.8.8           181
        4.8.7           180
        4.8.4           159

Midnight Commander (also known as mc) is a free cross-platform orthodox
file manager and a clone of Norton Commander.

Features include the ability work with common archive formats as if they
were simply another directory, and to function as an FTP. Midnight
Commander also includes an builtin editor called mcedit, features
include syntax highlighting for many languages, macros, code snippets,
simple integration with external tools, automatic indentation, mouse
support, clipboard and the ability to work in both ASCII and hex modes.

Midnight Commander can also rename groups of files, move files to a
different directory at the same time as it renames them. It lets the
user specify the original and resulting file names using wildcard
characters.

Midnight Commander is released under the GNU General Public License
version 3 or any later version. A copy of the file is included with this
distribution package.


Install
-------

Install simply though use of the windows installer package.

Default directories are as follows, available using the '-F' command
line option, the installation directory maybe be changed at your option:

 o Windows XP/Vista/7/8 and 10

   Config directory:
        C:/Program Files/Midnight Commander/etc/

   Data directory:
        C:/Program Files/Midnight Commander/share/

   VFS plugins and scripts:
       extfs.d:  C:/Program Files/Midnight Commander/plugin/extfs.d/
       magic:    C:/Program Files/Midnight Commander/etc//magic

   User data:
       C:/Documents and Settings/<user>/Application Data/Midnight Commander/

Once installed place the installation directory into your PATH. As an
alternative keeping your PATH and dll's namespace clean, create a simple
batch mc.bat which points to the true installation image.

Alternatively, a choco package is being maintained seperately yet this
version generally lags behind.

   https://chocolatey.org/packages/mc


Getting Started
---------------

There are a numerious resources detailing working with Midnight
Commander, including:


   o Midnight Commander Draft Documentation


        https://www.midnight-commander.org/wiki/doc

   o FAQ

        see 'docs' within the installation directory.


Resources
---------

Window native port for GNU Midnight Commander, the latest builds can be
found at the links:

   https://github.com/adamyg/mcwin32/ (master)

   https://sourceforge.net/projects/mcwin32/ (mirror)


Specific information regarding the base Midnight Commander 4.8.x engine,
can be found at the following

   http://en.wikipedia.org/wiki/Midnight_Commander

   www.midnight-commander.org


Midnight Commander Skin Editor

   https://phplego.github.io/mc/


Older information is available at

   www.gnu.org/software/mc


Status
------

I would consider this port stable, yet not all things may work as designed;
yet as this package is in use day-to-day expect issues to be addressed
quickly.

Please feel free to raise tickets on GitHub (preferred) or SourceForge when issues are encountered.

adamy
Sept/2023


Other Resources
---------------

There are a number of alternative, yet older, native builds available on
the web. The two most referenced are:

        o www.siegward-jaekel.de/mc-gb.html

        o franco-bez.4lima.de



Features and Limitations
------------------------

Internal editor is supported (including syntax highlighting).

Internal viewer is supported (including hex editor).

        Note the underlying the view logic may invoke one or more system
        utilities which are not generally available on Windows systems.

        If upon viewing a file using <F3> and it fails, use <shift-F3> which
        shall use the internal viewer bypassing the file extension based
        logic.

VFS (virtual file system) is enabled, yet not all of the modules have
been enabled.

Concurrent subshell is not supported.

Use forward slashes where possible, as backslash support is not fully
tested.

A few items are unix specific (e.g. chown), which shall be updated over
time.

-end-





