# How to run

- Make sure [Docker](https://www.docker.com/products/docker-desktop/) is installed and working on your system.
- Clone the repository: `git clone https://github.com/a-s-russo/sjx.git`.
- Switch to the `docker` branch: `git switch docker`.
- Build the Docker image using `docker build -t sjx_image .`
- Run the Docker container (and mount a volume) using `docker run --rm --name sjx_container -v /path/to/shared_folder:/home/sjx/shared_folder:rw sjx_image` (changing `/path/to/shared_folder` to a location on your computer).
- Inspect the contents of `shared_folder` for the output.
