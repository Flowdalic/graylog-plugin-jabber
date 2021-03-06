XMPP / Jabber Plugin for Graylog
================================

[![Build Status](https://travis-ci.org/Graylog2/graylog-plugin-jabber.svg?branch=master)](https://travis-ci.org/Graylog2/graylog-plugin-jabber)

XMPP/Jabber Alarmcallback Plugin for Graylog.

**Required Graylog version:** 1.1 and later

## Installation

[Download the plugin](https://github.com/Graylog2/graylog-plugin-jabber/releases)
and place the `.jar` file in your Graylog plugin directory. The plugin directory
is the `plugins/` folder relative from your `graylog-server` directory by default
and can be configured in your `graylog.conf` file.

Restart `graylog-server` and you are done.

## Build

This project is using Maven and requires Java 7 or higher.

You can build a plugin (JAR) with `mvn package`.

DEB and RPM packages can be build with `mvn jdeb:jdeb` and `mvn rpm:rpm` respectively.

## Plugin Release

We are using the maven release plugin:

```
$ mvn release:prepare
[...]
$ mvn release:perform
```

This sets the version numbers, creates a tag and pushes to GitHub. TravisCI will build the release artifacts and upload to GitHub automatically.
