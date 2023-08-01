# (.github/workflows/marlin.yaml) Build Marlin Firmwares

## Example

```yaml
name: ExampleService-DEV
on:
  push:
    branches: [main]
jobs:
  build:
    uses: aplaceformom/workflows/.github/workflows/.github/workflows/marlin.yaml@main
    with:
      output_obj: "Target filename of the firmware"
      config_dir: "The directory holding your configs"
      prefix: "Firmware prefix"
      artifact_key: "Artifact name to use"
```

## inputs

### marlin_branch

- **description**: Marlin branch to use
- **type**: string
- **default**: bugfix-2.1.x
- **required**: False

### build_env

- **description**: The build 'environment' to use
- **type**: string
- **default**: mega2560
- **required**: False

### build_obj

- **description**: The build object, or resulting firmware
- **type**: string
- **default**: NONE
- **required**: False

### output_obj

- **description**: Target filename of the firmware
- **type**: string
- **default**: False
- **required**: True

### config_dir

- **description**: The directory holding your configs
- **type**: string
- **default**: False
- **required**: True

### ini_dir

- **description**: The directory holding custom ini files for platformio
- **type**: string
- **default**: NONE
- **required**: False

### platformio_config

- **description**: The path and filename of the file to use as platformio.ini
- **type**: string
- **default**: NONE
- **required**: False

### flavor

- **description**: Flavor tag for the firmware
- **type**: string
- **default**: stock
- **required**: False

### prefix

- **description**: Firmware prefix
- **type**: string
- **default**: False
- **required**: True

### artifact_key

- **description**: Artifact name to use
- **type**: string
- **default**: False
- **required**: True

## secrets
