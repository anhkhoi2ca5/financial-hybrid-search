FROM mcr.microsoft.com/devcontainers/python:1-3.11-bookworm

# Remove the stale yarn apt source (its signing key is outdated and breaks apt-get update)
RUN for f in $(grep -rlE 'yarnpkg\.com' /etc/apt/sources.list.d/ 2>/dev/null); do rm -f "$f"; done
