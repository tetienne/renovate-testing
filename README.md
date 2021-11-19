# Minimal example for Gemfile without version constraint

This repo is used as a "minimal reproduction" for the discussion in renovatebot/renovate#7883

It illustrates an issue where a missing (or open ended) version contraint leads to no dependency updates from Renovate.
All gems defined in `Gemfile` are locked at older versions in `Gemfile.lock`.
This means that a successful Renovate run should create PRs for all gems.
