# Synthetic Adverse Events - Drugs ("SynthAERS")



My theory is that there is enough Open Data already available to create predictive models of how a particular new chemical compound may behave along the product development and marketing timeline.
Using prior (historical) data as a reference.


I already started building "Risk Profiles" of drugs
http://nihpo.com/wp-content/uploads/Oxaliplatin.xlsx
http://nihpo.com/wp-content/uploads/Ramucirumab.xlsx



As to your specific question: right now we assign a totally random adverse event to each record in the AE Domain.


In terms of future improvements (depending on resource availability):
* Create a table of all drugs licensed in the US / EU. (Done)
* Load entire FDA AERS / FAERS dataset in a local database. (Done)
* For each drug, indicate SOC.
* For each drug, indicate disease(s) approved for.
* For each drug, extract list of AEs reported in AERS / FAERS.
  => Compile table of AEs per drug, with frequency counts.

Then, use the AE frequency table when generating synthetic AEs.



# License Notice
Please note that this software is licensed under the [GNU AGPL](https://www.gnu.org/licenses/why-affero-gpl.html).

[Contact NIHPO](mailto:Jose.Lacal@NIHPO.com?subject=GitHub%20inquiry.) for a commercial license, or if you're interested in licensing a customized version of the NIHPO Synthetic Health Data Platform.

:copyright: 2007-2021 NIHPO, Inc.     Version 07 August 2021.