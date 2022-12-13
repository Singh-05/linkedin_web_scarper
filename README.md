# LinkedIn Web Scraper
Linkedin jobs web scraper in jupyter notebook
We are going to retrieve information about all available Data scientist jobs currently available in the Barcelona area. 

Results are shown in a "list form" and in different pages. For each job post there's also an additional page where more detailed information is provided.

Objective: Generate a DataFrame that contains the following information for all the listed job posts:

1. Job Title
2. Company Name
3. Location
4. State
5. Posting Date
6. Offer URL
7. Number of Applicants (in int form)
8. Promoted (in boolean form)
9. Workspace
10. Seniority
11. Employment Type
12. Industry
13. Python Required (in boolean form)
14. Application through Linkedin (in boolean form)
15. Number of Employees (in int form)


According to the following criteria:

In cases when values for any of the attributes above are not specified, the corresponding entries should be filled with pandas NaN values.  

The Job Titlte, Company Name and Location attributes should correspond to the basic offer information as displaye din both the short listing and the extended offer webpage.

The State attribute should be “Early Applications” if there is an alert that shows Early Applicant, "On-going" if there is an alert that shows Actively Hiring/Recruiting, or “Others” for alerts that are different than the two previously mentioned ones.

The Posting Date attribute should correspond to the time elapsed since the publication of the job offer (as displayed in the job post).

The Offer URL should correspond to the URL address for the more detailed job description page.

The Number of Applicants attribute should be stored in integer form. In some cases, you'll notice that the text "Be among the first 25 applicants" appears where the number of applications should be. For this case, the retrieved value should be 25.

The Promoted attribute should be encoded with a True if the job offer is Promoted and with a False otherwise.

The Workspace attribute should include information about whether the job offer is Hybrid, On-site , Remote or Other

The Seniority attribute should encode the level of the job, i.e. whether it's Entry, Mid-Senior, Senior, etc.

The Employment Type attribute should encode the work schedule, i.e. whether it's Full-time, Part-time, etc.

The Industry attribute should encode the sector of industry the company belongs to

The Python Required atribute should be equal to True if the word Python is mentioned in the Job Description (your check should not be case sensitive), or False if the word python is not mentioned in the Job Description.

In some cases, it is possible to apply for the job directly through LinkedIn using the Easy apply feature. In others, the offer will redirect you to the company's website where you can complete the applications process. The Application through Linkedin attribute should include a True whenever Easy apply is enabled and a False otherwise

The Number of Employees attribute should be stored in integer form and displayed the number of employees of the company offering the job. Should be filled by a pandas NaN when the company name is not specified, or the number of employees is not specified.

In all cases, strings should be properly formatted by removing any unnecessary spaces.
