# fitcli

**fitcli** is a command-line tool written in Go (Golang) designed for manipulating Garmin FIT files. It allows users to easily interact with FIT files, dumping their content, and integrates with various fitness platforms to upload and download files.

**Currently still under development. Not yet intended to be used**

## Features

- Parse and manipulate Garmin FIT files.
- Dump FIT file contents in a human-readable format.
- Integration with fitness platforms for file upload and download.
- Simple and intuitive command-line interface.

## Installation

To install **fitcli**, you need to have Go installed. You can install **fitcli** using the following steps:

### 1. Clone the repository:

```bash
git clone https://github.com/yourusername/fitcli.git
cd fitcli
```

### 2. Build the tool:
```bash
go build -o fitcli
This will produce a fitcli binary that you can use directly.
```

### 3. Install via Go (optional):
You can also install fitcli globally by running:

```bash
go install github.com/thesystemicprogrammer/fitcli@latest
```

This will install fitcli to your Go workspace's bin directory.

## Usage
Once installed, you can run fitcli directly from the command line.

### General Syntax:
```bash
fitcli [command] [flags]
```

### Commands:
- dump: Dumps the content of a FIT file in a human-readable format.

```bash
fitcli dump <filename>
```

- upload: Upload a FIT file to a fitness platform.

```bash
fitcli upload <filename> --platform <platform_name>
```

- download: Download a FIT file from a fitness platform.

```bash
fitcli download --platform <platform_name> --activity_id <id>
```

### Example Usage:
```bash
# Dump FIT file contents
fitcli dump my_activity.fit

# Upload FIT file to Strava
fitcli upload my_activity.fit --platform strava

# Download FIT file from TrainingPeaks
fitcli download --platform trainingpeaks --activity_id 123456
```

###  Supported Platforms
- XERT 
- Garmin Connect
 
## Contributing
Contributions are welcome! If you'd like to contribute to fitcli, please fork the repository, create a new branch, and submit a pull request.

Before submitting your changes, make sure to:

- Write tests for new features.
- Ensure all tests pass.
- Update the documentation if necessary.

## License
This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.
