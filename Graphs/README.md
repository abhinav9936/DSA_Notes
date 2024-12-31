# ISA XML Validator

## Overview

The **ISA XML Validator** is a tool designed to validate XML files for ISA (Instruction Set Architecture) compliance. It performs checks for completeness and correctness, generating detailed reports and logs.

## Pre-requisites

- No specific pre-requisites are required, but ensure that you have:
  - The XML files to validate.
  - The exclusion file, which specifies files or elements to exclude from validation.

## Usage

To run the tool, use the following command:

```bash
./validate-isa-xml.py [-h] --xml_file XML_FILE --exclusion_file EXCLUSION_FILE --working_dir WORKING_DIR [--no_color]

Arguments:
--xml_file XML_FILE (required): Path to the folder containing the XML files to be validated.
--exclusion_file EXCLUSION_FILE (required): Path to the exclusion file.
--working_dir WORKING_DIR (required): Path to the working directory where logs and reports will be stored.
--no_color (optional): Disables color output in the terminal.

Example:

./validate-isa-xml.py --xml_file /path/to/xml --exclusion_file /path/to/exclusion.xml --working_dir /path/to/working_dir --no_color
```

## Output

- Topdown-database and Bottomsup-database: These databases will be created inside the regression_dir folder, which is located inside the working_dir.
- Log Files: All the log files generated during validation will be stored in the regression_dir folder.
- Console Summary: A table will display the status and summary of each validation check on the console.
- Full Log: A detailed log of the validation process, including any failures, will be written to the output.result file inside the regression_dir.


## Clean-up

Before running the tool again, always ensure that the regression_dir folder is cleared to prevent interference from previous runs. This ensures that the new validation run starts with a clean slate.

## Debugging Information

During execution, the tool will display a table showing the name, status, and summary of each check.
In case of validation failures, the output.result file will contain detailed logs to assist with debugging.
More Information

For more details, please refer to https://confluence.arm.com/display/ATG/ISA+Decoder+validator+User+manual
