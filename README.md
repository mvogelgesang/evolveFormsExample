# SF Evolve Forms Demo

An implementation using [SF Evolve Forms](https://github.com/google/sf-evolve-forms/).

## Contents

- [SF Evolve Forms Demo](#sf-evolve-forms-demo)
  - [Contents](#contents)
  - [Setup](#setup)
    - [Cloning](#cloning)
    - [New Scratch Org](#new-scratch-org)
    - [Installation](#installation)
    - [Explore](#explore)
      - [Different Layout Options](#different-layout-options)
      - [Custom Components](#custom-components)
      - [Field Sections](#field-sections)

## Setup

### Cloning

The SF Evolve Forms project is included in this repo as a submodule. To fully clone the repo and the submodule, include the `--recurse-submodules` flag. Otherwise, the sf-evolve-forms folder will not contain anything.

`git clone git@github.com:mvogelgesang/evolveFormsExample.git --recurse-submodules`

### New Scratch Org

Skip to Install if you already have an org available.

Create a new scratch org and populate with data. Your scratch-def.json should include `"hasSampleData": true,` in the settings.

`sf org create scratch --target-dev-hub MyHub --definition-file config/project-scratch-def.json --set-default --duration-days 21`

### Installation

Deploy SF Evolve Forms directory
`sf project deploy start --source-dir sf-evolve-forms/evolve-forms/`

Deploy force-app directory
`sf project deploy start --source-dir force-app/`

### Explore

#### Different Layout Options

Account record pages display all three layout options (legacy, Dynamic Forms, SF Evolve)

#### Custom Components

Contact record pages offer a custom component that allows users to set a favorite color.

#### Field Sections

The Detail tab within Contact record pages demonstrate the use of field sections to group fields, customize labels, set required, and disabled.

In addition, a rich text area is included inbetween two field sections (you can also do this with Dynamic Forms).
