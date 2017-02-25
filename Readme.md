# Phoenix Vagrant Environment

Provides a ready-to-go environment for Phoenix development.

## Requirements

To get livereload to work in vagrant you need to install the
(vagrant-fsnotify)[https://github.com/adrienkohlbecker/vagrant-fsnotify] plugin
first.

```
vagrant plugin install vagrant-fsnotify
```

Then after you boot the VM make sure to run

```
vagrant fsnotify
```

to watch for changes.
