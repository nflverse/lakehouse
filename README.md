
<!-- README.md is generated from README.Rmd. Please edit that file -->

# nflverse-data

<!-- badges: start -->
<!-- badges: end -->

This repository holds automated data releases for nflverse projects
(i.e. all of the data powered/scraped via GitHub Actions).

## Usage

You can download data hosted here with the `{nflreadr}` package, or
manually download and access the
[releases](https://github.com/nflverse/nflverse-data/releases) page.
Releases are roughly organized along the [main
functions](https://nflreadr.nflverse.com/reference/) of nflreadr.

## Automation Status

The following table reports on the status and last update times of
nflverse data pipelines.

| Data               | Status                                                                                                                                                         | Last Updated                                                                                                                                                                                                                                                                                              |
|:-------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| pbp_raw            | []()                                                                                                                                                           | [![raw pbp data](https://img.shields.io/github/last-commit/nflverse/nflfastR-raw?label=Raw%20PBP%20Updated&style=flat-square)]()                                                                                                                                                                          |
| pbp                | [![pbp and ps](https://img.shields.io/github/workflow/status/nflverse/nflfastR-data/update_current_season_pbp_and_stats?label=pbp_status&style=flat-square)]() | [![pbp](https://img.shields.io/badge/dynamic/json?color=blue&label=load_pbp&query=last_updated&style=flat-square&url=https://github.com/nflverse/nflverse-data/releases/download/pbp/timestamp.json)](https://github.com/nflverse/nflverse-data/releases/tag/pbp)                                         |
| player_stats       | [![pbp and ps](https://img.shields.io/github/workflow/status/nflverse/nflfastR-data/update_current_season_pbp_and_stats?label=ps_status&style=flat-square)]()  | [![player_stats](https://img.shields.io/badge/dynamic/json?color=blue&label=load_player_stats&query=last_updated&style=flat-square&url=https://github.com/nflverse/nflverse-data/releases/download/player_stats/timestamp.json)](https://github.com/nflverse/nflverse-data/releases/tag/player_stats)     |
| rosters            | [![rosters](https://img.shields.io/github/workflow/status/nflverse/nflfastR-roster/update_rosters?label=rosters_status&style=flat-square)]()                   | [![rosters](https://img.shields.io/badge/dynamic/json?color=blue&label=load_rosters&query=last_updated&style=flat-square&url=https://github.com/nflverse/nflverse-data/releases/download/rosters/timestamp.json)](https://github.com/nflverse/nflverse-data/releases/tag/rosters)                         |
| snap_counts        | [![snap_counts](https://img.shields.io/github/workflow/status/nflverse/pfr_scrapR/update_snap_counts?label=snaps_status&style=flat-square)]()                  | [![snap_counts](https://img.shields.io/badge/dynamic/json?color=blue&label=load_snap_counts&query=last_updated&style=flat-square&url=https://github.com/nflverse/nflverse-data/releases/download/snap_counts/timestamp.json)](https://github.com/nflverse/nflverse-data/releases/tag/snap_counts)         |
| pfr_advstats       | [![adv_stats](https://img.shields.io/github/workflow/status/nflverse/pfr_scrapR/update_adv_stats?label=advstats_status&style=flat-square)]()                   | [![pfr_advstats](https://img.shields.io/badge/dynamic/json?color=blue&label=load_pfr_advstats&query=last_updated&style=flat-square&url=https://github.com/nflverse/nflverse-data/releases/download/pfr_advstats/timestamp.json)](https://github.com/nflverse/nflverse-data/releases/tag/pfr_advstats)     |
| nextgen_stats      | [![ngs](https://img.shields.io/github/workflow/status/nflverse/ngs-data/update_ngs?label=ngs_status&style=flat-square)]()                                      | [![nextgen_stats](https://img.shields.io/badge/dynamic/json?color=blue&label=load_nextgen_stats&query=last_updated&style=flat-square&url=https://github.com/nflverse/nflverse-data/releases/download/nextgen_stats/timestamp.json)](https://github.com/nflverse/nflverse-data/releases/tag/nextgen_stats) |
| injuries           | []()                                                                                                                                                           | [![injuries](https://img.shields.io/badge/dynamic/json?color=blue&label=load_injuries&query=last_updated&style=flat-square&url=https://github.com/nflverse/nflverse-data/releases/download/injuries/timestamp.json)](https://github.com/nflverse/nflverse-data/releases/tag/injuries)                     |
| depth_charts       | []()                                                                                                                                                           | [![depth_charts](https://img.shields.io/badge/dynamic/json?color=blue&label=load_depth_charts&query=last_updated&style=flat-square&url=https://github.com/nflverse/nflverse-data/releases/download/depth_charts/timestamp.json)](https://github.com/nflverse/nflverse-data/releases/tag/depth_charts)     |
| combine            | []()                                                                                                                                                           | [![combine](https://img.shields.io/badge/dynamic/json?color=blue&label=load_combine&query=last_updated&style=flat-square&url=https://github.com/nflverse/nflverse-data/releases/download/combine/timestamp.json)](https://github.com/nflverse/nflverse-data/releases/tag/combine)                         |
| nfl4th             | [![nfl4th](https://img.shields.io/github/workflow/status/nflverse/nfl4th/update-computed-numbers?label=nfl4th_precompute&style=flat-square)]()                 |                                                                                                                                                                                                                                                                                                           |
| ffverse player IDs | [![weekly-playerids](https://img.shields.io/github/workflow/status/dynastyprocess/data/weekly-playerids?label=ff_playerids&style=flat-square)]()               |                                                                                                                                                                                                                                                                                                           |
| ffverse rankings   | [![weekly-fantasypros](https://img.shields.io/github/workflow/status/dynastyprocess/data/weekly-fantasypros?label=rankings&style=flat-square)]()               |                                                                                                                                                                                                                                                                                                           |
