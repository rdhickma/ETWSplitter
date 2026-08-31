ETWSplitter

Simple program to split up large ETL files. Making them easier to process and handle. You can specify how many files you want to split the trace into or specify a time range to export. There is also optional compression.

Usage:
- Split mode:     ETWSplitter.exe <InputFile.etl> <OutputFile.etl> <#_of_Files> [compress]
- Time range mode: ETWSplitter.exe <InputFile.etl> <OutputFile.etl> -t <start_time>-<end_time> [compress]

Examples:
- ETWSplitter.exe input.etl output.etl 4
- ETWSplitter.exe input.etl output.etl -t 10-60
- ETWSplitter.exe input.etl output.etl -t 10-60 compress


Most of the magic happens in the Microsoft.Diagnostics.Tracing.TraceEvent library which you can find on Nuget.
https://www.nuget.org/packages/Microsoft.Diagnostics.Tracing.TraceEvent/

You can find a compiled ETWSplitter.exe in the Releases section.
