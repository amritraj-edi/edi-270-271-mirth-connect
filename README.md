# X12 270/271 EDI Mapping with Mirth Connect

## Overview
Portfolio demonstration of four Mirth Connect channel configurations for parsing ANSI X12 270 eligibility inquiry and 271 eligibility response transactions into CSV and XML outputs.

## Included
- `Channels/EDI270 to CSV Parsing.xml`
- `Channels/EDI270 to XML Parsing.xml`
- `Channels/EDI271 to CSV Parsing.xml`
- `Channels/EDI271 to XML Parsing.xml`
- Synthetic 270/271 text samples and blank CSV mapping templates

## Workflow
1. Receive a text-based X12 transaction.
2. Parse selected segments and elements in a Mirth Connect channel.
3. Map selected payer, provider, and subscriber/eligibility fields.
4. Produce CSV or XML output according to the channel mapping.

## How to review
Open the channel XML files in a compatible Mirth Connect environment and inspect the source/transformer/destination configuration. These are exported channel definitions, not a packaged Mirth deployment. Test them in a non-production environment with synthetic data before relying on the output.

## Data handling
Original sample/result files were intentionally not included because they contained realistic names, identifiers, addresses, and dates. Public examples in this repository are synthetic. Do not commit production EDI files, PHI, credentials, endpoint details, or client-specific configuration.

## Limitations
- This is a focused mapping exercise, not a complete X12 validator.
- Field coverage and business rules depend on the channel logic and the relevant trading-partner companion guide.
- CSV/XML outputs are mapping-specific representations, not universal canonical formats.
- Verify transaction structure, segment counts, delimiters, required fields, and expected results using approved test cases.

## Portfolio summary
Created Mirth Connect channel mappings to transform selected X12 270 eligibility inquiry and 271 eligibility response data into CSV and XML formats, using sample inputs and output templates to demonstrate parsing and data mapping.


