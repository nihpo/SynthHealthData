# NIHPO's Synthetic Health Data Platform

Lifesciences companies need access to unencumbered health data to accelerate their development, testing, and validation processes. Realistic, scientifically-valid yet synthetic health data can help shrink the regulatory approval timeline.

NIHPO’s Synthetic Health Data Platform helps *all staff roles* at *life sciences companies* to *reduce the time* it takes to 
* design, 
* develop, 
* test, 
* validate, and
* obtain regulatory approval for
new *drugs* and *medical devices*.

The Platform programmatically generates realistic, 100% scientifically correct, yet fully synthetic people ("SynthPerson").
For each SynthPerson the platform generates a complete synthetic Personal Health Record ("SynthPHR").
SynthPatients live in a series of geographically-accurate synthetic cities ("SynthCity"). 
SynthPatients are then randomly selected to participate in synthetic Clinical Trials ("SynthTrials"). 
Platform users define the parameters of a clinical trial and the platform generates all SDTM domains for the desired number of subjects.
Once the Synthetic Trial is generated, users can build the equivalent of a full digital Synthetic Submission ("SynthSubmission") to a Health Agency.


NIHPO's Synthetic Health Data Platform:
[SynthPHR](/synthphr) => [SynthEDC](/synthedc) => [SynthImaging](/synthimaging) => [SynthTrial](/synthtrial) => [SynthSubmission](/synthsubmission)

In this repository you can analyze and download the Python-based software that powers this platform.





Sponsor:
* Developing software to test clinical trial data.

Software developer:
* “Not being part of a pharma company I do not have access to clinical trial data.”

CRO. 
* “We need data to speed up development of systems.”
* Creation of test data => speed up data sets?
* Starting point: “we can’t use clients’ data.”

Requirements:
* Must be conformant to latest CDISC standard.




## Create Unencumbered Synthetic Health Data at Scale

The synthetic data this platform generates is:
* 100% scientifically valid (LOINC, SNOMED-CT)
* Includes Real World Data (devices; drugs; US providers)

Synthetic data significantly reduces time to:
* Test, validate trial software
* Predict, solve trial data issues early
* Compile trial data into full submission
* "Walk" SynthPatients through SynthTrials
* Perform end-to-end test, QA, validation


## The Problem we Solve
Access to realistic, unencumbered health data:
* Before real clinical trial data becomes available
* Assist during clinical
* Software Development
* Software Testing: Fuzz Testing, corner cases
* Shorten Quality Assurance cycles
* Crucial for end-to-end System Validation

With no copyright, legal, privacy, regulatory blocks.

## Who has This Problem?
* Pharmaceutical companies (“Sponsors”)
* Clinical Research Organizations (“CROs”)
* Hospitals testing inter-operability, migrations 
* Health IT providers / vendors
* Regulatory Agencies
* Software developers

NIHPO is working towards a full, end-to-end “Computable Clinical Trial Data Platform”


## Stage I: Synthetic Personal Health Records

User can generate Synthetic Personal Health Records ("SynthPHRs") on demand, at scale.

User can create synthetic cohorts at will: assign gender distribution; define age ranges; select countries; include / exclude pre-existing disease types; etc.

The generated SynthPHR files can be downloaded.

![Synthethic PHR diagram](SynthHealthData_01.png)

Please see the [SynthPHR](/synthphr) section for more details.



## Stage II: Synthetic Clinical Trial

User runs the pre-generated synthetic cohorts through a Synthetic Clinical Trial.

Select a pre-defined "Synthetic PHR" created above, define a clinical trial (arms, phases, visits, etc.), and "run" the cohort through the trial.
User will be able to re-run the same cohort through as many trials as needed.

The system generates the full output for a trial (CDISC-formatted files, in both CSV and SAS format).

The generated SynthTrial files can be downloaded.

![Synthetic Trial diagram](SynthHealthData_02.png)

Please see the [SynthTrial](/synthtrial) section for more details.


## Stage III: Synthetic Clinical Trial Submission

User selects a pre-defined SynthTrial and builds a Docker container with a full "Computable Clinical Trial Submission".

The Docker container includes all the CDISC SDTM files, plus the SynthPHRs, plus other files we're working on.

* Fully digital trial data submission 
* Reviewer analyzes full raw data 
* Runs in self-contained Virtual Machine / Docker image
* Greatly reduce time to approval

![Synthetic Submission diagram](SynthHealthData_03.png)

Please see the [SynthSubmission](/synthsubmission) section for more details.

Users will be able to boot the Docker container in Azure, as a full self-contained regulatory submission.

![Azure hosting Synthetic Submissions](SynthHealthData_04.png)


## Stage IV: Synthetic Electronic Data Capture ("SynthEDC")

We're exploring the business value of building synthetic, unencumbered Electronic Data Capture ("EDC") datasets at scale.

Please see the [SynthEDC](/synthedc) section for more details.


## Stage V: Synthetic Medical Imaging ("SynthImaging")

There seems to be a scarcity of scientifically-valid yet synthetic medical images.

We're exploring the business value of building synthetic, unencumbered Electronic Data Capture ("EDC") datasets at scale.

Please see the [SynthImaging](/synthimaging) section for more details.


## User Benefits

Imagine this: a user will be able to go from zero to a fully computable (synthetic) regulatory submission in under an hour.

Accessible through a web browser, hosted in Azure, with no IT intervention.

How many hours of drudgery and copy-and-paste work can we save to staffers in medical device and Pharma companies? 


# Why Open Source our Intellectual Property?

NIHPO has consciously decided to publish its software's source code under the [GNU AGPL](https://www.gnu.org/licenses/why-affero-gpl.html) license from the Free Software Foundation.

At NIHPO, we define ourselves as Data Artistes. We love Open Data, and our passion is turning Open Data into actionable knowledge.

Like artists everywhere, the greatest impediment to our success is when nobody knows about our art. We want every person who could benefit from our software to be free to try the software, in their own terms, with neither financial nor legal barriers.

We believe that by demonstrating both our art and our passion for this craft, upfront and with no restrictions, we'll be able to attract subscribers willing to pay us to enhance and customize the software we're providing here for free.

We're following the [Product-led Growth](https://www.productled.org/foundations/what-is-product-led-growth) strategy. We believe that the quality of our product, and that you can try it before you buy it, will open doors for us.


# License Notice
Please note that this software is licensed under the [GNU AGPL](https://www.gnu.org/licenses/why-affero-gpl.html).

[Contact NIHPO](mailto:Jose.Lacal@NIHPO.com?subject=GitHub%20inquiry.) for a commercial license, or if you're interested in licensing a customized version of this platform.

:copyright: 2007-2021 NIHPO, Inc.     Version 01 April 2021.