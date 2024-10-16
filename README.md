# PHP Docker Apache MariaDB PHP-Compose

## Setup

### Direnv
This template uses [direnv|https://direnv.net] for managing environment and secrets (for development only).

Ensure direnv is installed on your computer, and started or added to your shell-startup script (`~/.bashrc` oder `~/.zsh_rc`).
When you first enter this directory allow the use of direnv: `direnv allow`.
After altering the direnv file you need to allow it again to ensure no bad behavior where implemented, please check beforehand.

Copy the `.secrets.env.example` to `.secrets.env` and set the values for your setup.  

### Project files

Project files are placed in `src/` and the `public`-directory is the apache default directory within the `src/` directory.
This is the default for the most common frameworks, if you need to modify the htdocs-root dir, please modify this in the `.env` file.


### docker

To start the docker container (for development) simply use: `docker-compose up`.

