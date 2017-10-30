# Gzdec gstreamer plugin

## It's a work in progress Gstreamer plugin

It's a test in order to develope one viable Gstreamer plugin capable of uncompress files compressed using gzip and bzip.

When finished it would be fully compatible with Gstreamer-1.0 and Gstreamer-0.10 but for know only Gstreamer-1.0 is contemplated in the provisory code.

For know it doesn't do anything.

## Installation:

In order to install the plugin you need to do this:

./autogen.sh
sudo make && sudo make install


In autogen.sh the default location is /usr/local. You would need to add /usr/local/lib/gstreamer-1.0 to GST_PLUGIN_PATH or edit the path in the autogen.sh file in order to make make the new plugin show up in a Gstreamer that's been installed from packages.

You would also need to install the zlib.h and bzlib.h just in case it's no present in your system:

sudo apt-get install zlib1g-dev

sudo apt-get install libbz2-dev
