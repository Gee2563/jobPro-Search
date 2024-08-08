# jobPro-Search
Chrome extension that auto-fills job details to JobPro's tracker on 3rd part sites.

The logic:

jobPro-Search scans a page's content for key-words that have a score associated to them. When the website's keyword score is greater or equal to the target score, chrome prompts you
if you are applying for a job. if yes, it will attempt to store the information in the following JSON format:
{
job: {
CompanyName: -,
CompanyWebsite: -,
JobTitle: -,
Description: -,
etc..,
dump: -,
}
}

The object would then be stored automatically to the applied section in jobPro's application tracker in the Active/researching stage.
From the app, you'd be able to tailor your CV and generate cover letters. If straightforward, the jP-Search will generate a tailored CV directly on the application's website.

If for some reason it fails to find attributes, such as jobTitle, it will dump the data in job.dump for the user to manually breakdown or description.

