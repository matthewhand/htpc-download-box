
# Project Status Report

## Date
2023-06-15

## Completed Tasks

1. Set up the default Noteable project and created a new notebook.
2. Shut down the kernel for the previous notebook to ensure available kernel resources.
3. Created and updated files in the GitHub repository using the PyGitHub module.
4. Set up the following services using Docker Compose:
   - Jackett
   - Plex
   - Tautulli
   - Portainer
   - Watchtower
   - WireGuard

## Next Steps

1. Check the status of the Docker services on the local machine or server.
2. If any of the services are not running, check their logs for any error messages.
3. Continue with the next tasks in the TODO list.

## Challenges

1. We're working in a Jupyter notebook environment, so we don't have the necessary permissions to start Docker services or check their status. These tasks need to be done on the local machine or server.
2. We have limited kernels in Noteable, so we need to avoid creating new notebooks.

## Learnings

1. We can use the PyGitHub module to interact with GitHub repositories from a Python notebook.
2. We can use Docker Compose to set up multiple services with a single configuration file.
