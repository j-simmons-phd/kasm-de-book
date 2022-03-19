# Digital Engineering Book Development Kasm Workspace

## Introduction

This repo provides a Kasm Workspace for developing the definitive text on the practice of Digital Engineering.  This text will be developed following a model-based approach.  The tools in the development workspace will be selected to support this approach.   It includes the following tools.

- git cli
- [Keychain](https://www.funtoo.org/Keychain)
- [Obsidian](https://obsidian.md/) and [JabRef](https://www.jabref.org/) for note taking
- Chrome
- [Evince Document Reader](https://wiki.gnome.org/Apps/Evince) 
- [Pandoc](https://pandoc.org/)
- [yq](https://mikefarah.gitbook.io/yq/) v4.20.2

## A Note on Licensing

This repo includes code and packages from a number of outside sources (including [Kasm Workspaces](https://www.kasmweb.com/)).  The project license file only covers code written by the project author and contributors.  All other code is subject to its authors' terms and conditions.

## How to Use this Repo

1. Download and unzip the latest release
1. Open the unzipped release folder in the command line 
1. Run `docker-compose pull` to download the image 

## Using the image locally

Once downloaded, the image can be pushed into the Kasm server per Kasm documentation or it can be run locally on port 6901 using docker-compose.

- **Starting the image locally:** Run `docker-compose up -d`
- **Stopping the image locally:** Run `docker-compose down`

When running locally, the workspace can be accessed at https://localhost:6901 with
- **User:** `kasm_user`
- **Passwordd:** `password`
