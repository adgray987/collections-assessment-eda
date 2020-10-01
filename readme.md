
# Collections Assessmenet Exploratory Analysis

A notebook for exploratory analysis of archival collections assessment data using Pandas.

## Explanation
Assessments can hold valuable data about collections that can be [leveraged in different contexts](https://www.oclc.org/content/dam/research/publications/library/2011/2011-07.pdf) (strategic planning, surfacing hidden collections, etc.). This notebook uses basic Pandas functionality to clean and do an exploratory analysis of assessment data from an ArchivesSpace Assessment record list report, and to answer a few example questions about a fictional repository:

- How are the collection survey sizes distributed?
- How much material needs to be reformatted?
- What kind of condition are these collections in?
- What are the major at-risk formats in the assessed collections?
- Which collections contain specific formats?

While the example analysis focuses on using the assessment data to inform digitization/reformatting decisions, it could just as easily focus on using the data to inform other areas of practice, such as processing to improve discoverability and preservation needs assessments. This notebook only scratches the surface of how Pandas can be used in scalable, reproducable solutions to advance data-informed decision-making and produce new knowledge from collections (meta)data. 

## Data Source
The record list report used in this notebook is populated with fake data. It is modeled on a [vanilla assessment import template ](https://github.com/archivesspace/archivesspace/blob/master/backend/app/exporters/examples/assessment/aspace_assessment_import_template.csv) from the ArchiveSpace Assessment module, so it is should be fairly straightforward to repurpose for reports for real repositories. It can also be adapted to explore assessment data in ANY spreadsheet, not just those from ASpace - just modify the code to suit your column headers and data types.

## Requirements

- Pandas
- Numpy

For an introduction to Pandas, the [official documentation](https://pandas.pydata.org/pandas-docs/stable/getting_started/index.html) is a good place to start.

## Can't I just do this in Excel and/or OpenRefine?

If all you need to do is clean up a few free-text fields and apply some filters, those tools are great! But programmatic cleaning and analysis with Pandas is much easier to replicate when new assessments are performed and when assessment records are updated, allowing for more efficient tracking of changes in collection conditions and progress toward strategic goals. This means you can use Pandas to do more with less time and effort.
