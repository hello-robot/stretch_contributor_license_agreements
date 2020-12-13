## How do I contribute to Hello Robot's official repositiories?

Please download and sign the individual or entity PDF file found in this repository, depending on whether you are contributing as an individual or as part of an organization. After signing the PDF, please email it as an attachment to info@hello-robot.com . Hello Robot Inc. will review the document. If Hello Robot Inc. agrees to the terms, a final signed copy will be emailed back to you.

## Why does Hello Robot ask contributors to sign contributor license agreements (CLAs)?

Hello Robot Inc. values the community forming around the Stretch mobile manipulator. We welcome interest in contributing to the materials we have released. Since we are working to build a company that will stand the test of time, we require contributor license agreements (CLAs) from individuals and entities who wish to contribute to the company repositories.

Hello Robot Inc. uses a variety of [Open Source Initiative (OSI)](https://opensource.org/licenses) approved licenses. Hello Robot Inc. reserves the right to dual license these materials. This provides a method by which Hello Robot Inc. can serve businesses with distinct licensing requirements. For us to accept contributions to the official materials from an individual or entity outside of Hello Robot Inc., the individual or entity must sign a contributor license agreement (CLA) found within this repository. 

## How did Hello Robot create these agreements? 

We first generated contributor license agreements (CLAs) with http://contributoragreements.org/ by selecting "Create Custom CLA" and "Option 5 - No commitment to any specific outbound license." and "Traditional Patent License". We then made minor edits to the resulting markdown files. 

## How did Hello Robot generate the PDFs from the markdown files? 

We used command line tools in Ubuntu 18.04.

We first installed pandoc with the following commands. 

```
sudo apt install pandoc
sudo apt install texlive-fonts-recommended
```

We then used the following commands to generate the PDF files.

```
pandoc -V geometry:margin=1in -s hello_robot_individual_cla_20201212.md -o hello_robot_individual_cla_20201212.pdf 
pandoc -V geometry:margin=1in -s hello_robot_entity_cla_20201212.md -o hello_robot_entity_cla_20201212.pdf
```

