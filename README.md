# ![The Swedish Pathogens Portal](static/img/swe_pathogens_logo.png)

# The Swedish COVID-19 Sample Collection Database

This is the source code for the [Swedish COVID-19 Sample Collection Database](https://biobanks.pathogens.se), part of the [Swedish Pathogens Portal](https://pathogens.se). The database is maintained in collaboration with [Biobank Sverige](https://biobanksverige.se/).

The site is built using the [Hugo](https://gohugo.io/) static web site generator.
In addition, it uses [Bootstrap 4](https://getbootstrap.com/), [Font Awesome](https://fontawesome.com), [DataTables](https://datatables.net/).

Re-use of our code to run other similar databases is welcome as long as the license conditions are met. Importantly, we note that the code shared here comes with no guarantees that it works or that it works well.

## Introduction: formats and structure

The database contains two types of entries: biobanks and sample collections. Each sample collection is nested under a particular biobank. Information about both biobanks and sample collections is stored in YAML format (with extention `*.md`), making it easy to edit.

All biobanks currently in the database can be found in the folder `/content/collections/`. Folder names here correspond to the biobank registration number at *Inspektionen för vård och omsorg, IVO* (English: *The Swedish Health and Social Care Inspectorate*). Within each biobank folder, the file `_index.md` contains information about the biobanks (such as the name, acronym, juridical person, contact info, etc.)

Within each biobank folder, the files named `1.md`, `2.md`, etc. contain information about sample collections belonging to that particular biobank.

## Editing information about existing biobanks and sample collections

The easiest way to edit information about an existing biobank or sample collection is to do so using on the GitHub website.

### Step 1: Access the code

The code is hosted on [GitHub](http://github.com/), so you'll need an account.

Next, visit the code repository: [https://github.com/ScilifelabDataCentre/covid-sample-collection-database](https://github.com/ScilifelabDataCentre/covid-sample-collection-database)

In the top right, you'll see a button that says _"Fork"_. Click this, then select your username. This makes a copy of the repository under your personal account that you can edit.

### Step 2: Edit the files

On the web page of your _forked_ copy of the repository, look in the `content/collections/` directory.

Note also that the filenames correspond to the website URL:

- [https://biobanks.pathogens.se/collections/325/1/](https://biobanks.pathogens.se/collections/325/1/)
    - `content/collections/325/1.md`
- [https://biobanks.pathogens.se/collections/325/](https://biobanks.pathogens.se/collections/325/)
    - `content/collections/325/_index.md`

Go to the markdown file that you want to edit, then click the Pencil icon :pencil2: in the top right.
This opens a web-based editor where you can add and edit content.

When you're finished, scroll to the bottom and fill in / submit the _"Commit changes"_ form.

You're nearly done.

### Step 3: Make a pull request

Once you're finished with your edits and they are committed and pushed to your forked repository, it's time to open a pull request.

You can find full documentation on the [GitHub help website](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests), however in short:

- Visit the main repository: [https://github.com/ScilifelabDataCentre/covid-sample-collection-database](https://github.com/ScilifelabDataCentre/covid-sample-collection-database)
- Click the button that reads _"New Pull Request"_
- Click the text link near the top that says _"compare across forks"_
- In the right-hand _"head repository"_ drop down, select your username / fork.
- If you're happy with the list of commits shown, and the diff in the _"Files Changed"_ tab, fill in a title and description and click _"Create pull request"_

Once created, a member of the website team will review your changes.
Once approved, they will be merged and deployed.

## How to get help

If in doubt, you can ask for help by emailing [datacentre@scilifelab.se](mailto:datacentre@scilifelab.se).

## Credits

The website was built by [SciLifeLab Data Centre](https://www.scilifelab.se/data/).
