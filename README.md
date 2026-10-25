# Richman — txAdmin custom template

This small public repository contains the txAdmin recipe for the Richman
Russian-language GTA V Enhanced server. It installs a minimal Cfx baseline and
sets game build 3407. It does not include the private server source, player
data, bridge implementation, or credentials; it does not yet install the
planned Foundry-agent NPC resource.

## Import into txAdmin

In txAdmin's Server Deployer, import this recipe URL:

`https://raw.githubusercontent.com/pastfama/richman-public/main/recipe.yaml`

The recipe is intended for a **new/empty deployment target**. Do not run it as
an update against the live Richman profile: it creates a baseline resources
tree and writes `server.cfg`.

txAdmin prompts for the Cfx license and deployment options; no credentials are
stored in this repository. See the private Richman project documentation for
the server's operational details.

## Source of truth

The canonical recipe is maintained in the private `pastfama/Richman` repository
at `infra/txadmin-richman-enhanced.yaml`. A GitHub Actions workflow publishes
only this recipe and this README into this public repository. Do not edit the
generated copy here; propose changes in the private source repo.