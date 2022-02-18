# Digital Engineering Book Development Kasm Workspace

## Introduction

This repo provides a Kasm Workspace for developing the definitive text on the practice of Digital Engineering.  This text will be developed following a model-based approach.  The tools in the development workspace will be selected to support this approach.   It includes the following tools.

- git cli
- [Keychain](https://www.funtoo.org/Keychain)
- Emacs with support for [Org-roam](https://www.orgroam.com/) to facillitate a model-based approach to research and note taking
- Chrome
- [Evince Document Reader](https://wiki.gnome.org/Apps/Evince) 
- [Pandoc](https://pandoc.org/)

## How to Use this Repo

1. Clone this repo, giving the new repo a descriptive name for the workspace image to be created
1. Run `docker-compose build` to build the workspace image (see [Issue #1](https://github.com/j-simmons-phd/kasm-core-focal-template/issues/1) if you encounter an error in Step 1/15 for manual steps to correct the issue).  Note, debugging build errors is easier when you switch the docker-compose [progress mode](https://docs.docker.com/engine/reference/commandline/compose_build/#options) to plain (`docker-compose build --progress plain`)

## Using the image locally

Once built, the image can be pushed into the Kasm server per Kasm documentation or it can be run locally on port 6901 using docker-compose.

- **Starting the image locally:** Run `docker-compose up -d`
- **Stopping the image locally:** Run `docker-compose down`

When running locally, the workspace can be accessed at https://localhost:6901 with
- **User:** `kasm_user`
- **Passwordd:** `password`
