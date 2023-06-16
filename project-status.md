
    # Project Status Report

    ## Date
    2023-06-16

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
    5. Updated the TODO list in the GitHub repository.

    ## Next Steps

    1. Resolve the issue with `sudo` not being able to run as root in the current container environment.
    2. Install MicroK8s.
    3. Add the worker nodes to the MicroK8s cluster.
    4. Deploy various Helm charts to the cluster, including Grafana, Prometheus, Dashboard, and Netbox.

    ## Challenges

    1. We're working in a Jupyter notebook environment, so we don't have the necessary permissions to start Docker services or check their status. These tasks need to be done on the local machine or server.
    2. We have limited kernels in Noteable, so we need to avoid creating new notebooks.
    3. The current environment does not allow `sudo` to run as root, which is necessary for the installation of MicroK8s.

    ## Learnings

    1. We can use the PyGitHub module to interact with GitHub repositories from a Python notebook.
    2. We can use Docker Compose to set up multiple services with a single configuration file.
    