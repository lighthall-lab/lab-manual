# Lab Resources

## Slack

Slack will be used as the primary means of lab communication, such as general lab announcements (`#-general`), sharing links, sharing and/or discussing papers (`#-papers`), and basically any message that can be sent without email. There's also a channel for keeping notes from our lab meetings (`#-lab-meetings`), as well as channels for specific projects (e.g. `#econdec`).

Try to keep each channel on topic, so that people can subscribe only to the channels that concern them. For messages to one person or a small group of people, use the direct message channels. Because we pay per Slack user, part-time RAs will be invited as "guests" to the `#undergrads` channel; these users can also use direct messages.

Full-time lab members should install Slack to their computers and/or phones. Part-time lab members should check Slack regularly. I get Slack updates on my phone and have do-not-disturb mode enabled for evening and night hours (meaning I will not get your messages then); I encourage you to do the same.

## Email
When it's appropriate to use email instead of Slack, such as when there is a lot to say at once or a long-form one-on-one discussion, such as negotiating lab hours, etc., feel free to do so. We also have a lab email account that goes to only the lab manager(s) and PhD students: `lighthall-lab@gmail.com`.

## GitHub

All projects that involve programming of any kind must use some form of version control. We have a [GitHub organization](https://github.com/lighthall-lab/) set up, allowing you to sync your code to the cloud and share it easily with other lab members.

Hosted on the lab's GitHub, you'll find a tutorial repository on the basics of using git for version control, and there is a `#-github` channel in Slack for questions, sharing, and discussion. We will also use GitHub for sharing script examples and hosting lab toolboxes for general use.

## Google Calendar

Google Calendar is used to host a general lab calendar (AD&D Lab), as well as calendars for the in-lab testing rooms.

## Google Drive

The AD&D Lab folder on Google Drive is used to store documents and files for general lab use (e.g., IRB documents, stimuli, pdfs, etc). It can also be used for some forms of non-identifiable [data](#data-management).

## Research Drive
The "Research Drive" is our **secure UCF server** that houses all of our experiments, including stimuli, data, and analyses. You should have full access to this drive once the lab managers have completed your orientation and onboarding procedures, and it should appear as the R:/ drive on any of the lab's IT-managed computers.

### Accessing the Research Drive 
Your personal computers are also capable of accessing this data, so long as you are connected to the `UCF_WPA2` wireless network, or use the [UCF VPN](https://www.cst.ucf.edu/wp-content/uploads/service%20desk/NewVPN_user.pdf) to connect to the university network from home. When connected to the UCF network, you can access the Research Drive in two ways:
- Direct Navigation
	- In your computer's file browser, type the address directly into the address bar:
		- `\\net1110.net.ucf.edu\research2\lighthall_lab\`
	- Sign in with your UCF NID and NID password
- Mount as a Network Drive
	- Windows
		1. Right click on "This PC" and select "Map network drive..."
		2. Choose a drive letter (We use "R:") and enter the server address:
			- `\\net1110.net.ucf.edu\research2\lighthall_lab\`
	- Mac
		1. ***[to-add]**: instructions for mounting network share on Mac OS
		
### Structure of the Research Drive
I encourage you to become very familiar the Research Drive's directory structure - you will be accessing it quite often. Our allocation is structured like this:
- `_archive`
  - For old stimuli, datasets, analyses, out-of-date code, or anything else that's not being used anymore.
  - Deleting files from the Research Drive cannot be undone (*there's no "Recycle Bin"!*), so moving things here that you don't need anymore is the preferred method for disposal unless you are **1000% sure** you won't need it anymore.
  - This stuff is first on the chopping block when we need to save space on the Research Drive.
- `_working`
  - For stuff you're - *drumroll, please!* - working on, that doesn't quite belong anywhere else.
- `apps`
  - Source code for various code toolboxes and utilities you may need to use.
  - You might be pointed here if you need to use one of the ones we already store here, but you are also welcome to store anything here in its own directory if you think you and/or others might find it useful.
  - If you do find a package or utility you want to store here, put it here in its own directory using `git clone` or another method, and feel free to work on it here.
- `docs`
  - `user`
    - For any small files and documents you're working on for yourself that you need somewhere to store, feel free to create a folder in here with your name/initals/whatever.
    - Please don't abuse this storage by putting large files in here. Anything you put in here is also viewable to anyone else with access to the Research Drive, so don't store any sensitive or confidential information here.
  - `resources`
    - Tutorials, templates, recruitment materials, forms, etc., for example:
    - `lab-manual`
    - `guides`
      - `Git-Version-Control-Tutorial`
      - `Image Processing`
    - `textbooks`
    - `papers`
    - `meetings`
    - `llrn`
      - Resources for the *Learning & Longevity Research Network*
- `experiments`
  - Individual folders for each project, with structure like so:
  - `project-name`
    - `docs`
      - `protocol`
      - `irb`
    - `deploy` 
      - Shortcuts, numbered and clearly named, in the order they appear on the study's exam protocol, pointed at the necessary files in `stimuli`, for easy deployment at the time of data collection.
    - `stimuli`
      - All stimuli should be stored here: stimulus images, paradigm scripts, configuration files, etc. When appropriate, such as when the `deploy` directory shortcuts are not working, the experiment should be run directly from these files. 
    - `sourcedata`
      - All raw datafiles created by the experiment paradigm when data is collected, in individual subject folders.
      - Unless absolutely necessary, we should *never* directly manipulate the structure or content of datasets here. Instead, we should develop pipelines (`code`) for extracting data from here, transforming it, and loading it into `derivatives`.
      - The preferred structure for datasets is the [BIDS](http://bids.neuroimaging.io/) standard structure with individual folders for each subject:
        - `sub-101`
        - `sub-102`
        - `sub-201`
          - `beh`
          - `anat`
          - `func`
    - `code`
      - All code being used to extract, clean, merge, transform, analyze, etc., any of the project's data should be stored here, and kept as organized and tidy as possible, containing a README.md file that describes as much info as possible about the study and pipeline.
      - Code organization and tidyness might include giving your files descriptive, concise names, sorting pipeline steps into folders, appending your filenames with step numbers (e.g., `1.extract.sh`,`2.tranform.py`), etc.
      - This directory should always be a local git repository pointed to a remote repository origin on the [Lab GitHub](https://github.com/lighthall-lab/")
    - `derivatives`
      - All analysis files, intermediary data transformations, figures, etc., should go here.
      - Data pipelines should only **ever** write data into this folder or its subfolders, and should be kept well-organized and tidy just as the `code` is.
      
