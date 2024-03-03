# SaviEg

## Overview

SaviEg is designed to parse SAS EG Projects and extract their contents. It is written in C# under .NET 8+.

## Architecture

SaviEg.exe is compiled as x64 and as a single exe. Please install .NET 8 before using.

## Parameters

To see the available parameters, execute SaviEg with a /? or a --help at the command line. This will display the help for the commands.

## Reports

SaviEg generates a simple summary report that can be found in the Work directory after processing. 

## Logging

All parsing logs are written to the user temp path (%temp%) and are under the directory *Savian\SaviEg*

## Sample call

.\SaviEg.exe --MaxLogSize 1000000 --Output "C:\temp\SaviEgOut" --Path "[C:\temp\EgProjects; X:\repos\EgProjects]" --Work "C:\temp\SaviEgWork"
