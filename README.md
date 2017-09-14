# spectrum-schematics-cluster

Schematics is a template system for IBM Bluemix based on terraform

This repository can be cloned or directly used in IBM Bluemix Schematics. You simply provide your account info and ssh keys, you can also fine controll with other terraform variables

## Release Information

* IBM Spectrum Symphony Cluster on Schematics
* Supported Product: symphony v7.2.0.0

## Contents

* Introduction
* Usage
* Release Notes
* Community Contribution
* Copyright
 
## Introduction

To use IBM schematics, you need to gain certain information, here is the most important ones

- ibm_bmx_api_key
  - your api key for IBM Bluemix
  - If you do not have an existing API key, you can generate the value by running bluemix iam api-key-create NAME
- ibm_sl_username
  - your username for SoftLayer
- ibm_sl_api_key
  - your api key for SoftLayer
  - You can retrieve the value from the "SoftLayer Customer Portal", in the API Access Information section
- ssh_public_key
  - your personal ssh public key to access servers on softlayer
  - you need to have "manage sshkey" permission on bluemix

## Usage

### steps

- login to IBM bluemix, navigate to Schematics
- create new environment
  - Source Control URL: use this repository or your forked repository 
  - Variables (required)
    - ibm_bmx_api_key
    - ibm_sl_username
    - ibm_sl_api_key
    - ssh_public_key
  - Variables (optional)
    - refer to the file terraform.tfvars
- plan and view plan log
- apply and view apply log

### all variables

- please read terraform.tfvars and/or main.tf

## Release Notes

### Release initial

- This is the first release from IBM Spectrum Computing.
- Create centos based symphony 7.2.0.0 virtual machines on SoftLayer using Schematics.
- Required variables
  - ibm_bmx_api_key
  - ibm_sl_username
  - ibm_sl_api_key
  - ssh_public_key

## Community Contribution Requirements

Community contributions to this repository must follow the [IBM Developer's Certificate of Origin (DCO)](https://github.com/IBMSpectrumComputing/platform-python-lsf-api/blob/master/IBMDCO.md) process and only through GitHub Pull Requests:

 1. Contributor proposes new code to community.

 2. Contributor signs off on contributions 
    (i.e. attachs the DCO to ensure contributor is either the code 
    originator or has rights to publish. The template of the DCO is included in
    this package).
 
 3. IBM Spectrum LSF development reviews contribution to check for:
    i)  Applicability and relevancy of functional content 
    ii) Any obvious issues

 4. If accepted, posts contribution. If rejected, work goes back to contributor and is not merged.

## Copyright

### Unlicense

This is free and unencumbered software released into the public domain.

Anyone is free to copy, modify, publish, use, compile, sell, or
distribute this software, either in source code form or as a compiled
binary, for any purpose, commercial or non-commercial, and by any
means.

In jurisdictions that recognize copyright laws, the author or authors
of this software dedicate any and all copyright interest in the
software to the public domain. We make this dedication for the benefit
of the public at large and to the detriment of our heirs and
successors. We intend this dedication to be an overt act of
relinquishment in perpetuity of all present and future rights to this
software under copyright law.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.

For more information, please refer to <https://unlicense.org>
