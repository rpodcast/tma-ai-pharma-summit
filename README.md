## Trusted Mini-Agents 

This repository contains the materials of the presentation **Guardrails, Not Guesswork: Harnessing the Power of AI Responsibly with Trusted Mini-Agents** shared during the Validated AI for Pharma Summit (2026-09-24)

* Slides authored by Will Landau are available in the `assets` folder of this repository.
* Example Shiny application performing a basic clinical trial simulation using the trusted mini-agents workflow. This application is copied from the upstream trusted mini-agents guide available at <https://trustedminiagents.dev>.

## Development Setup

If you wish to run the Shiny application on your system, you can do so using the following procedure:

* Install the Nix Package Manager using the Determinant Systems installer for your operating system: <https://determinate.systems/posts/determinate-nix-installer>
* Clone this repository to your system.
* Navigate to the root of this repository and build the Nix environment by running `nix-build` in a terminal.
* Update the `new_chat` function located in the `R/tools.R` script to use your preferred AI provider supported by `{ellmber}`. In this repository, the Open Router service is used for the AI provider. You will need to create a new `.Renviron` file in the root of this repository. An example is provided in the `.Renviron.example` file.
