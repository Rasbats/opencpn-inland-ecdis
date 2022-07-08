## Building the main manual

The manual can be built locally or published on Github Pages

### Publish to Github Pages

Push the current branch to the branch *build*, something like

    $ git push -f origin HEAD:build

The results becomes available at https://github.com/opencpn-manuals/main
after about 3-4  minutes.

### Local builds

Local builds requires Nodejs and npm installed. See
https://docs.antora.org/antora/3.0/install/install-antora/,
but note that the antora program does not need to be installed.
Just nodejs and npm is enough.

The preparation step is to install required npm modules:

    $ npm install

After completing this step, documentation is built using

    $ npm run build

The resulting site can  be viewed by directing a browser to
_docs/index.html_.

### UI bundle

The UI bundle used is forked from the default Antora UI bundle.
Sources: https://gitlab.com/leamas/antora-ui-default
