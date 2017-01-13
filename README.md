# Build pack to setup headers for building ruby-filemagic

This buildpak simply adds in the headers and lib symlink for the already installed libmagic so that ruby-filemagic can be installed.

Simply add this to your chain of buildpaks before heroku/ruby to use.

## NOTE

This wil output a warning by the heroku/ruby buildpak about a .bundle/config existing. This is how the headers and lib are configured so that bundle/rubygems can find libmagic.

