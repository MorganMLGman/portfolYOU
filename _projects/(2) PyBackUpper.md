---
name: PyBackUpper
tools: [Python, Docker, Linux]
image: /assets/pybackupper.png
description: PyBackUpper is simple Python application deployed with Docker container. It's main goal is to create daily backups of server, but can be used to backup pretty much anything you like.
---

# PyBackUpper

<p class="text-center">
{% include elements/button.html link="https://github.com/MorganMLGman/PyBackUpper" text="Go see on GitHub" %}
</p>

PyBackUpper is a simple Python application created to make backups of self-hosted server based on Docker, but could be used to create any kind of backups. For time of writing, the application can create backups at specified time of the day and specified days of the week. Application create a copy of the source directory at a given time and preserve directory owner, group and permissions. It is also possible to compress created backup with to `.tar.gz` archive. Backups will be deleted from disk after a given amount of runs, for example if you specify to run a backup every second day and keep 7 runs, the first backup will be deleted after two weeks.

![preview](/assets/pybackupper.png)

## Features
- Creating backups at specified time of the day
- Creating backups at specified days of the week
- Compressing created backups to `.tar` archive. Currently only `.tar.gz` but there will be more
- Deleting old backups
- Preserving owner, group and permissions
- Created `.tar` archive can be created with given owner and group
- Skipping files matching given pattern, like `*.log`
