# Reconfigure locales

select the locales you want in the list (with your settings, you need en_GB and en_US.UTF-8
I recommend selecting en_US and en_GB.UTF-8 as well)

```bash
dpkg-reconfigure locales
```

# Installed locales

```bash
locale -a
```

There you should see `en_US.utf8` or `en_US.UTF-8`

# Locale Variables

```bash
locale
```

Should show:

```bash
LANG=en_US.utf8
LANGUAGE=en_US:en
LC_CTYPE="en_US.utf8"
LC_NUMERIC="en_US.utf8"
LC_TIME="en_US.utf8"
LC_COLLATE="en_US.utf8"
LC_MONETARY="en_US.utf8"
LC_MESSAGES="en_US.utf8"
LC_PAPER="en_US.utf8"
LC_NAME="en_US.utf8"
LC_ADDRESS="en_US.utf8"
LC_TELEPHONE="en_US.utf8"
LC_MEASUREMENT="en_US.utf8"
LC_IDENTIFICATION="en_US.utf8"
LC_ALL=en_US.utf8
```

# Reinstall language pack

```bash
apt-get install --reinstall language-pack-en
```

# Set locale variables
especially if you have an error/warning like this
`locale: Cannot set LC_ALL to default locale: No such file or directory`
`perl: warning: Setting locale failed.`

```bash
export LC_ALL="en_US.utf8"
```

