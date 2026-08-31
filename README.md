ETWSplitter

Simple program to split up large ETL files. Making them easier to process and handle.

So I found the Microsoft.Diagnostics.Tracing.TraceEvent library which you can find on Nuget.
https://www.nuget.org/packages/Microsoft.Diagnostics.Tracing.TraceEvent/

Usage:
- Split mode:     ETWSplitter.exe <InputFile.etl> <OutputFile.etl> <#_of_Files> [compress]
- Time range mode: ETWSplitter.exe <InputFile.etl> <OutputFile.etl> -t <timestart>-<timeend> [compress]

Examples:
- ETWSplitter.exe input.etl output.etl 4
- ETWSplitter.exe input.etl output.etl -t 10-60
- ETWSplitter.exe input.etl output.etl -t 10-60 compress


There is optional compression you can use too.

You can find a compiled ETWSplitter.exe in the Releases section.
