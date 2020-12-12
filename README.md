# Why do we ask contributors to sign contributor license agreements?

Hello Robot Inc. values the community forming around the Stretch mobile manipulator. We welcome interest in contributing to the materials we have released. Since we are working to build a company that will stand the test of time, we require contributor license agreements (CLAs) from individuals and entities who wish to contribute to the company repositories.

Hello Robot Inc. uses a variety of [Open Source Initiative (OSI)](https://opensource.org/licenses) approved licenses. Hello Robot Inc. reserves the right to dual license these materials. This provides a method by which Hello Robot Inc. can serve businesses with distinct licensing requirements. For us to accept contributions to materials that we have released, individuals and entities must sign a contributor license agreement (CLA) found within this repository. 

# How did we created these agreements? 

We first generated contributor license agreements (CLAs) with http://contributoragreements.org/ by selecting "Create Custom CLA" and "Option 5 - No commitment to any specific outbound license." and "Traditional Patent License". We then made minor edits to the resulting markdown files. 

# How did we generate the PDFs from the markdown files? 

We used command line tools in Ubuntu 18.04.

We first installed pandoc with the following commands. 

```
sudo apt install pandoc
sudo apt install texlive-fonts-recommended
```

Then we then used the following commands to generate the PDF files.

```
pandoc -V geometry:margin=1in -s hello_robot_individual_cla_20201212.md -o hello_robot_individual_cla_20201212.pdf 
pandoc -V geometry:margin=1in -s hello_robot_entity_cla_20201212.md -o hello_robot_entity_cla_20201212.pdf
```

