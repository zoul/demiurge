# About

This is a Perl script that replaces [imgur](http://imgur.com) links in your files with other URLs. It also downloads the referenced images, so it’s perfect for migrating your images off imgur.

# Running

    $ find . -name '*.md' -print0 \
        | xargs -0 demiurge --replacement-url=http://i.zmotula.cz

This will find replace all imgur links in your Markdown documents with images in the `http://i.zmotula.cz` domain. The images will be downloaded to the `images` folder so that you can upload them to your new server.

See the source for other command-line switches.