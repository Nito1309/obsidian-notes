
Configures any packages that are unpacked but not yet configured.
```
dpkg --configure --pending
```


Removes all files from the /var/cache/apt/archives/ directory, except the lock file. This directory is where apt stores downloaded package files.

```
apt-get clean
```

Updates the list of available packages and their versions.
```
apt-get update
```

Performs the functions of upgrade but also handles changing dependencies with new versions of packages.
```
apt-get dist-upgrade -o APT::Get::allow-downgrades=yes -o APT::Get::Assume-Yes=yes -o APT::Get::Ignore-Hold=yes -o APT::Get::Purge=yes -o APT::Get::Remove=yes
```
- -o APT::Get::allow-downgrades=yes: Allows downgrading of packages.
- -o APT::Get::Assume-Yes=yes: Assumes "yes" to all prompts.
- -o APT::Get::Ignore-Hold=yes: Ignores packages on hold.
- -o APT::Get::Purge=yes: Purges removed packages.
- -o APT::Get::Remove=yes: Removes packages that are no longer needed.

