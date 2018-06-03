git-kindle
==========

This is the simple tool to generate e-book for Amazon Kindle (in .mobi format) from git repository tree.

INSTALL
=======

This tool depends on [kindlegen][1] and [highlight][2]. This differs from upstream, which uses [source-highlight][3]. You need to download
kindlegen binary from [Amazon.com site][1]. As for highlight you can install it using the instructions from the [author's website][2].

Next you need to install script itself. Assuming you have `$HOME/bin` in your PATH:

    curl https://raw.githubusercontent.com/InnocentSmith0934/git-kindle/master/git-kindle > $HOME/bin/git-kindle
    chmod a+x $HOME/bin/git-kindle

USAGE
=====

Go to your repository directory (e.g. myproj) and run

    git kindle

It will search C files by default and create myproj.mobi file in current directory. You can also
specify custom regexp for file filter:

    git kindle '\.rb$'


[1]: http://www.amazon.com/gp/feature.html?docId=1000234621
[2]: http://www.andre-simon.de/doku/highlight/en/install.php
[3]: http://www.gnu.org/software/src-highlite/source-highlight.html#Download

