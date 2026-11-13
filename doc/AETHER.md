# Aether - build and release notes

## Channel and version
- Channel name: set at configure time, e.g. `autobuild configure -A 64 -c ReleaseFS_open -- --chan Aether`
- Version: `indra/newview/VIEWER_VERSION.txt`.
- Release notes: the viewer opens `<RELEASE_NOTES_BASE_URL><version>`, i.e.
  `https://github.com/Alistar-Snook/phoenix-firestorm/releases/tag/<version>`.
  Create a GitHub release with a tag equal to the version string for every build.

## Crash reports (BugSplat)
1. Create your own account/database on https://www.bugsplat.com (free tier available).
2. Configure with `-DBUGSPLAT_DB=<your_database_name>` (see `cmake/bugsplat.cmake`).
3. Upload symbols (PDB) for each release to the same database.
Builds without `BUGSPLAT_DB` (e.g. `ReleaseFS_open`) send no crash reports.

## Central data server (FSData)
Disabled: `FSDataBaseURL` is empty. If you host `data.xml`, `agents.xml` and `assets.xml`, set
`FSDataBaseURL` in `settings.xml` to enable it.

## Attribution
Source files keep their original copyright and license headers (LGPL 2.1). The About floater
keeps the Linden Lab / Firestorm / contributors credits. Do not use the Second Life or Firestorm
trademarks as the name of this viewer; follow the Second Life Third-Party Viewer Policy.
