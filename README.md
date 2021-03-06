# libnmap

## Code status

[![Build Status](https://travis-ci.org/savon-noir/python-libnmap.png?branch=master)](https://travis-ci.org/savon-noir/python-libnmap)

## Use cases

libnmap is a python library enabling python developpers to manipulate nmap process and data.
libnmap is what you were looking for if you need to implement the following:
- automate or schedule nmap scans on a regular basis
- manipulate nmap scans results to do reporting for instance
- compare and diff nmap scans to generate graphs for instance
- batch process scan reports
- ...

The above uses cases will be easy to implement with the help of the libnmap modules

## libnmap modules

The lib currently offers the following modules:

- process: enables you to launch nmap scans
- parse: enables you to parse nmap reports or scan results (only XML so far) from a file, a string,...
- report: enables you to manipulate a parsed scan result and de/serialize scan results in a json format
- diff: enables you to see what changed between two scans
- common: contains basic nmap objects like NmapHost and NmapService. It is to note that each object can be "diff()ed" with another similar object.
- plugins: enables you to support datastores for your scan results directly in the "NmapReport" object from report module
    - mongodb: only plugin implemented so far, ultra basic, for POC purpose only
    - sqlalchemy: on-going
    - csv: todo (easy to implement)
    - elastic search: todo

## Documentation

All the documentation is available on [read the docs](<https://libnmap.readthedocs.org>). This documentation contains small code samples that you directly reuse. 

## Examples

Some codes samples are available in the examples directory or in the [documentation](<https://libnmap.readthedocs.org>).
