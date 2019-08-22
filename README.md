# Google Summer of Code 2019 - "IPP Test Suite for IPP System Service"
The repository contains the code created for the project IPP Test Suite for IPP System Service during the Google Summer of Code 2019, under the aegis of **The Linux Foundation**.

## Overview - Existing tools and technologies
The section briefly describes the relevant Printer Working Group (PWG) tools and technologies.

#### Internet Printing Protocol (IPP)
 The Internet Printing Protocol is a ubiquitous application level protocol that enables communication between Application Program Clients and Printing Resources (or the Print Server) over a local network or the Internet. The protocol is supported by all modern network printers and supercedes legacy protocols.
 
 The client can perform tasks like querying the printer capabilities, status, submit mutliple print jobs, receive job status and cancel print jobs. The protocol also enables security capabilities like authentication,access control and encryption.
 
#### IPP Tool
IPP Tool is a program that sends IPP requests to the specified printer-uri and tests and/or displays the results based on requests by a testfile. The results include the expected response status, attributes, and values. Output is either a plain text, formatted text, CSV,or XML report on the standard output.

#### IPP System Service
IPP System Service is an organization-wide framework being developed by the Printer Working Group that acts as a central service to manage and control all the printing, scanning resources on the network under one roof. It enables clients to store common resources like static images, strings, template printer objects, administratively manage access controls on printing resources. This makes doing system wide changes easy and tractable.

#### IPP Tool Test-File
An ipptoolfile is a file that satisfies a predefined syntax and contains all information to be included in a request to be issued to a printer by ipptool. Apart from that, it also includes information to be expected in a response from the printer.

## Project Work
Pull request for my code into the **ippsample** repository can be found here: 

This repository contains the test-suite, that is a set of ipptest-files to check the conformance of a given system with the IPP System Service Standards. System managers can use these test-files to verify the status of different components like system,printers and resources under different system operations.

I have written test files for the following 


## Future Work
-Changing the test scripts according to the parser support for some data-types for the "OF-TYPE" predicate of the ipptool-file

-Change scripts to adjust to any changes in the ipptool program which supports dynamic (runtime dependent variable) testing

-Include COUNT predicate wherever necessary (TBD ASAP)

## Acknowledgements
I would like to extend my heart-felt gratitude to Mr. Michael Sweet, who helped me through all of the technical difficulties encountered in this project. Needless to say, without his guidance, none of this work would have been possible. I would also like to thank my mentors Ira McDonald, Danny Brennan, Till Kamppeter and Aveek Basu. I would also like to specially thank Aveek for his administrative, technical and moral support throughout my journey at the Open Prinitng Division of Linux Foundation.

## Conclusion
Google Summer of Code 2019 has been a unique experience and has helped me understand the workings of the Open-Source Industry. It has made me all the more confident in my abilities to make fruitful contributions to Open Source in the future. I would like to thank Google for providing this wonderful opportunity that helped me spend my Summers in the best way possible!


