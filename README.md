# Ruby 2.1.4 for Debian ARMHF

This repo contains debian packages for installing ruby 2.1.4 on an armhf device, such as a Beaglebone Black.

There are two packages:

* `ruby_2.1.4_armhf.deb` - installs to `/usr`
* `ruby_2.1.4-local_armhf.deb` - installs to `/usr/local`

# Not using debian?

If you just want the armhf ruby build you can do the following commands to extract them out of the debian package:

```sh
mkdir ruby-armhf
ar p ruby_2.1.4_armhf.deb | tar xzf - -C ruby-armhf

# install it straight to root
# ar p ruby_2.1.4_armhf.deb | tar xzf - -C /
```

Then you will find all the files in the `ruby-armhf` folder.
