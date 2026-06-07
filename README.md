[![licensebadge](https://img.shields.io/badge/license-MIT-blue)](https://choosealicense.com/licenses/mit/)

<!-- START Adjust URL -->
[![Solution passing all tests](https://img.shields.io/github/actions/workflow/status/Blockly2Java/ArrayBootcamp/test-solution.yml?branch=main&label=Solution%20passing%20all%20tests)](https://github.com/Blockly2Java/ArrayBootcamp/actions/workflows/test-solution.yml)
[![ArrayBootcamp compiling successfully](https://img.shields.io/github/actions/workflow/status/Blockly2Java/ArrayBootcamp/test-template.yml?branch=main&label=ArrayBootcamp%20compiling%20successfully)](https://github.com/Blockly2Java/ArrayBootcamp/actions/workflows/test-template.yml)
<!-- END Adjust URL -->

## Abstract

<!-- START Adjust for exercise -->
This exercise introduces fundamental operations on Java arrays. Students practice creating arrays, accessing elements by index, iterating over array contents, modifying array elements, and computing aggregate values. The seven tasks progressively build array proficiency — from basic declaration and element access to traversal and accumulation patterns.
<!-- END Adjust for exercise -->

Detailed exercise instructions can be found in the README file of the template repository.

## Local Setup

To set up the workspace for local development:

1. Clone this repository into a new folder:
   ```bash
   git clone git@github.com:Blockly2Java/ArrayBootcamp.git MyExercise
   ```
2. Navigate into the cloned folder and run the setup script:
   ```bash
   cd MyExercise
   ./local-setup.sh
   ```

The script will automatically restructure the directory layout:
- Moves this repository (with its git history) into a `parent/` subdirectory.
- Copies IDE settings and configuration files from `root-template/` to the workspace root.
- Clones/updates the sibling repositories (`template`, `solution`, `tests`) alongside `parent/`.

Resulting folder structure:
```text
MyExercise/
├── VS-Code.code-workspace  # Copied from root-template
├── parent/                 # This repository (git repo)
├── template/               # Student code template (git repo)
├── solution/               # Reference solution (git repo)
└── tests/                  # Test harness (git repo)
```

## Exporting to Artemis

This repository generates a ZIP file that can be directly imported into Artemis.

### Local Export


1. Ensure the workspace is set up (run `./local-setup.sh` if needed)
2. Run the export command: `<exercise-name>` must match the Repository-Name
   ```bash
   ./parent/.github/scripts/local-export.sh --name <exercise-name>
   ```

3. The ZIP file is created in the `Artemis_Export/` directory
4. Import the ZIP into Artemis via the exercise creation/edit UI

### GitHub Export

The export runs automatically on GitHub when code is pushed to any branch. Download the generated ZIP from the workflow artifacts and import it into Artemis.
