This file contains a general outline of the structure of atopile

.
├── 📂 assets/: Contains static assets like images used in documentation (e.g., README).
├── 📄 atopile-custom-words.txt: Likely a custom dictionary for spell checking specific to the atopile domain.
├── 📄 configured_for.yaml: Configuration file, possibly indicating what the current checkout or environment is configured for (e.g., specific hardware or features).
├── 📄 cspell.json: Configuration file for the cspell spell checker.
├── 📂 dist/: This is where build artifacts or distributable versions of atopile are placed.
│   └── 📄 (empty or build specific files like wheels or executables)
├── 📂 dockerfiles/: Contains Dockerfiles for creating containerized environments for atopile development or execution.
├── 📂 examples/: Contains example projects and files demonstrating how to use atopile.
│   ├── 📄 ato.yaml: Example project configuration for atopile.
│   ├── 📄 ch1_0_quickstart.ato: Example atopile design file.
│   ├── ... (other .ato, .py example files)
│   └── 📄 README.md: Provides an overview and instructions for the examples.
├── 📄 goose_prompt.md: System prompt or configuration for an AI assistant (Goose).
├── 📄 LICENSE: Contains the software license for the atopile project.
├── 📄 pyproject.toml: Standard Python project configuration file (PEP 518), specifying build system requirements and project metadata.
├── 📄 README.md: The main introductory document for the atopile project.
├── 📂 scripts/: Contains utility scripts for development, build, or maintenance tasks.
│   ├── 📄 attach_license.py: Script to add license headers to files.
│   ├── 📄 clean_issues.py: Script possibly for managing or cleaning up issue tracker data.
│   └── 📄 find_duplicate_test_files.sh: Shell script to find duplicate test files.
├── 📂 src/: Contains the source code for the atopile project.
│   ├── 📂 atopile/: Core source code for the atopile language, compiler, and toolchain.
│   │   ├── 📄 address.py: Likely handles addressing or locating elements within a design.
│   │   ├── 📄 attributes.py: Manages attributes of design components.
│   │   ├── 📄 buildutil.py: Utilities for the build process.
│   │   ├── 📂 cli/: Source code for the Command Line Interface.
│   │   ├── 📄 config.py: Handles configuration loading and management.
│   │   ├── 📄 datatypes.py: Defines custom data types used in atopile.
│   │   ├── 📄 errors.py: Defines custom error types and handling.
│   │   ├── 📄 front_end.py: Handles the initial parsing and processing of atopile code.
│   │   ├── 📄 __init__.py: Makes the directory a Python package.
│   │   ├── 📂 kicad_plugin/: Plugin for integration with KiCad EDA software.
│   │   ├── 📄 layout.py: Code related to PCB layout generation or processing.
│   │   ├── 📂 lsp/: Source code for the Language Server Protocol implementation, enabling IDE features.
│   │   ├── 📄 __main__.py: Entry point for the atopile application when run as a module.
│   │   ├── 📄 parse.py: Core parsing logic.
│   │   ├── 📂 parser/: Likely contains more detailed parser components (e.g., ANTLR generated code).
│   │   ├── 📄 parse_utils.py: Utility functions for parsing.
│   │   ├── 📂 project-template/: Template files for new atopile projects.
│   │   ├── 📄 telemetry.py: Handles telemetry data collection.
│   │   └── 📄 version.py: Manages version information for atopile.
│   └── 📂 faebryk/: Source code for Faebryk, possibly a related library or framework used by atopile.
│       ├── 📂 core/: Core components of Faebryk.
│       ├── 📂 exporters/: Modules for exporting Faebryk data to other formats.
│       ├── 📂 importers/: Modules for importing data into Faebryk.
│       ├── 📄 __init__.py: Makes the directory a Python package.
│       ├── 📂 library/: Contains a library of Faebryk components or modules.
│       ├── 📂 libs/: Other supporting libraries for Faebryk.
│       └── 📂 tools/: Utility tools specific to Faebryk.
├── 📄 structure.md: This file! Outlines the directory structure of the project.
├── 📄 telemetry.yaml: Configuration file for telemetry.
├── 📂 test/: Contains automated tests for the atopile codebase.
│   ├── 📂 cli/: Tests for the Command Line Interface.
│   ├── 📂 common/: Common utilities or fixtures for tests.
│   ├── 📄 conftest.py: Pytest configuration file, often contains shared fixtures.
│   ├── 📂 core/: Tests for the core logic of atopile.
│   ├── 📂 end_to_end/: End-to-end tests simulating user workflows.
│   ├── 📂 exporters/: Tests for exporter functionalities.
│   ├── 📂 front_end/: Tests for the front-end parsing.
│   ├── 📄 __init__.py: Makes the directory a Python package.
│   ├── 📂 integration/: Integration tests for different parts of the system.
│   ├── 📂 library/: Tests for the component library.
│   ├── 📂 libs/: Tests for supporting libraries.
│   ├── 📄 runpytest.sh: Shell script to run pytest.
│   ├── 📄 runtest.py: Python script for running tests.
│   ├── 📄 test_address.py: Tests for address.py.
│   ├── ... (other specific test_*.py files)
│   └── 📄 test_version.py: Tests for version.py.
├── 📂 tools/: Contains various tools for developers or users of atopile.
│   ├── 📂 atopile_mkdocs_plugin/: A MkDocs plugin specific to atopile for documentation generation.
│   ├── 📄 docs-sync.js: JavaScript file, possibly for synchronizing documentation or related tasks.
│   ├── 📂 library/: Tools related to the component library.
│   └── 📄 profile.py: Script for profiling atopile's performance.
└── 📄 uv.lock: Lock file for the `uv` Python package installer and resolver, ensuring reproducible builds.
