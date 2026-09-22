# Rekba — update feed

This repository holds nothing but the update manifests for
[Rekba](https://ibraverse.ca/projects/rekba/), a bus, tram and metro app for
Algeria. The installed app fetches these files to find out whether a newer
version exists.

| File | When the app reads it |
|---|---|
| [`AppCastCritical.xml`](AppCastCritical.xml) | A release the user must take — a broken timetable or a security fix. The app blocks until it is installed. |
| [`AppCastNotCritical.xml`](AppCastNotCritical.xml) | An ordinary release. The app mentions it and carries on. |

Both are [Sparkle](https://sparkle-project.org/) appcast feeds: an RSS channel
whose `<enclosure>` carries the version and the store link.

The repository is public because the app has to reach it without credentials.
The app itself is not open source — the project write-up is at
[ibraverse.ca/projects/rekba](https://ibraverse.ca/projects/rekba/).
