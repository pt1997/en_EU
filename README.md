# en_EU
Inofficial English locale for European (en_150)

this is intended for Linux users that want to use the English language.

It uses €, the same thousand separators as English, 24 Clock, YYYY-MM-DD.

You should probably use the current version of https://github.com/wyx227/glibc/blob/f9a3c7691852f2521439a94e1c1a1f8309a8655a/localedata/locales/en_EU


# how to use:

* download the en_EU file you want to use and move it to /usr/share/i18n/locales/en_EU

* install the `glibc-locale-source` or `locales` package using your package manager (depending on your distro) 

* run the following commands:
  ```
  sudo localedef -i en_EU -f UTF-8 en_EU.UTF-8
  localectl set-locale en_EU.UTF-8
  reboot
  ```

# why
most programs are written in with English in mind. All English locales have their problems for me and apparently many people

* https://unix.stackexchange.com/questions/62316/why-is-there-no-euro-english-locale
* https://askubuntu.com/questions/579267/support-for-en-150-locale
* https://sourceware.org/bugzilla/show_bug.cgi?id=22535
* https://sourceware.org/bugzilla/show_bug.cgi?id=22473
* https://sourceware.org/legacy-ml/libc-alpha/2017-08/msg00830.html
