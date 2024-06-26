# Synthetic Medicare ("SynthMedicare")

I'd like to build a "Synthetic Medicare Population" platform using Synthea.
The goal is to build a realistic, highly accurate model to represent the Medicare population as of the end of 2017.


With these inputs:

a.) Medicare (HHS CMS) provides data on "Medicare Provider Utilization and Payment Data"
https://www.cms.gov/Research-Statistics-Data-and-Systems/Statistics-Trends-and-Reports/Medicare-Provider-Charge-Data

The PUF data represents a baseline ("Real World Data") of who the Medicare patients actually are; their healthcare expenditures; and the providers who treat those patients. Including:
    Providers’ Patient Profile (age, gender, conditions)
    Prescription patterns (what Provider prescribes which drugs)
    Inpatient expenses
    Outpatient expenses
    Durable Medical Equipment expenses

b.) Add payments from medical device and pharma companies.
[https://www.cms.gov/OpenPayments]

c.) Add adverse event reports for drugs and devices during those years.

d.) Deploy the Synthetic Patients geographically, using each Provider's physical practice address.

e.) Generate the full medical record for each Synthetic Medicare Patient using the data from a.) above (in terms of incidence of disease, treatment patterns, drug consumption patterns, etc.
Start with each listed Provider and build as many Patients as the Provider reports in the PUF tables (yes, many Medicare patients go to multiple Providers, I need to start somewhere while staying purely within the Open Data space).


Once the platform is built above, then we can perform simulations and projections: impact of new drugs, new devices, etc. 





Stage 05: Medicare reimbursements.
* Analyze who (individual Medicare providers) prescribes each drug in
the target disease.
* Build geographical models of prescription patterns.
Sources: Medicare's PUF data.
{As you already know, Medicare is the single largest payer of
pharmaceutical products and healthcare services in the US}.





# License Notice
Please note that this software is licensed under the [GNU AGPL](https://www.gnu.org/licenses/why-affero-gpl.html).

[Contact NIHPO](mailto:Jose.Lacal@NIHPO.com?subject=GitHub%20inquiry.) for a commercial license, or if you're interested in licensing a customized version of the NIHPO Synthetic Health Data Platform.

:copyright: 2007-2021 NIHPO, Inc.     Version 07 August 2021.