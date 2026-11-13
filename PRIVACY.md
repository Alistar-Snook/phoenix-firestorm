# Aether privacy notice

Aether is a third-party viewer for Second Life based on the Linden Lab viewer and the
Firestorm viewer (LGPL 2.1). It is not affiliated with or endorsed by Linden Research, Inc.
or The Phoenix Firestorm Project, Inc.

- Aether does not download data from any central Aether server by default (`FSDataBaseURL` is empty).
- Crash reports are sent only if the build was configured with a crash-report database
  (`-DBUGSPLAT_DB=<name>`) **and** you leave "Send crash reports" enabled in
  Preferences > Network & Files > Crash reports. Reports contain technical data about the crash
  (call stack, OS, graphics hardware, viewer version) and may include your log file.
- Aether connects to Second Life (or the grid you choose) and to the login page of that grid.

Maintainers: update this file with the name and contact of the party operating the crash-report
database before publishing builds.
