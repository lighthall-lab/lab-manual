# General policies
## Hours
One of the benefits of a career in academic research is that it is typically more flexible than other kinds of jobs. However, you should still treat it like a job. If you are employed for 40 hours a week, you should be working 40 hours a week. This applies to lab staff members (the lab manager and other research assistants) and postdocs. You are not required to work over-time. For graduate students, I recognize that you have other demands on your time like classes and TA-ing but still expect to see you in lab, doing research, often.

Lab staff members are expected to keep regular office hours (e.g., somewhere in the ballpark of 9a-5p). Graduate students and postdocs have more flexibility. However, in order to encourage lab interaction, I expect that all lab members will be in the lab, at minimum, 10 hours per week.

### PI office hours
In addition to poking my head into the lab regularly, I will be in my office with the door open for at least an hour every day that I'm on campus (most days). Feel free to interrupt me during that time. Because I am easily distracted, I ask that if my door is closed, send me a message or try me later rather than knock.

## Meetings
### Weekly lab meetings
Weekly lab meetings will be focused on project presentations and going over new data or methods. Lab meetings will last no longer than 1 hour. If at the end of 1 hour, we need more time to discuss something, we will either take a break before continuing or schedule another meeting. Lab meeting agendas and notes will be maintained in the `#lab-meetings` channel on Slack. All full-time lab members are expected to attend the weekly lab meeting. All part-time lab members (including undergraduates) are welcome to attend but attendance is not required.
### Individual meetings
At the beginning of each semester, I will set a schedule to meet with each full-time lab member for one hour a week. If we do not have anything to discuss in a given week, that's fine; we can just say hi or cancel it.
### Journal clubs & Lab meetings
We will alternate between having a biweekly **lab meeting** and a biweekly **journal club**. Lab meeting topics will include project presentations, article discussions, and practice talks. The journal club will be focused on discussing new and/or important research articles. Some weeks, we'll discuss a single article that everyone has read; other weeks, we'll each read a paper on a specific theme and do mini-presentations on each paper. Journal club topics will be set in the `#papers` channel on Slack.

As with our internal lab meetings, all full-time lab members are expected to attend, and part-time lab members are invited but not required to attend.

## Deadlines
If you need something from me by a particular deadline, please inform me as soon as you are aware of the deadline so that I can allocate my time as efficiently as possible. I will expect at least one week's notice, but I greatly prefer two weeks' notice. I will *require* two weeks' notice for letters of recommendation. If you do not adhere to these guidelines, I may not be able to meet your deadline. Please note that this applies to reading/ commenting on abstracts, papers, and manuscripts, in addition to filling out paperwork, etc.

## Presentations
I encourage you to seek out opportunities to present your research to the department, research community, or general public. If you are going to give a presentation (including posters and talks), please be prepared to give a practice presentation to the lab at least one week ahead of time. Not only will this help you feel comfortable with the presentation, it will give you time to implement any feedback. I care about practice presentations because a) presenting your work is a huge part of being successful in science and it's important that you practice those skills as often as possible, and b) you are going to be representing not only yourself but also the rest of the lab.

There is a lab template for posters that you are free to modify as you see fit, but the header and general aesthetic should stay similar. If you have ideas for how to improve the poster template, please show the lab so we can decide whether to implement them as a group. This will help increase the visibility of our lab at conferences. (Don't believe me? Check out the various lab "walls" at the next conference you attend.) There is no template for talks, and I encourage you to use your own style of presentation as long as it is polished and clear.

### A note on colors
The PRC is red,<br>
the PHC is blue.<br>
All other colors<br>
are up to you.<br>

## Lab travel
The lab will typically pay for full-time lab members to present their work at major conferences (e.g., SFN, CNS, CEMS). In general, the work should be "new" in that it has not been presented previously, and it should be appropriate for the conference. When I set our grant budgets, I estimate $1500 per trip, so your reimbursable costs should be around that amount or less. Meal costs will be reimbursed for people who are presenting work from the lab. The lab will also pay for new grad students and postdocs to attend one conference in their first year in lab. If travel expenses are being paid off of a grant, additional restrictions may apply (talk to me). All of these guidelines, of course, depend on the availability of funds.

## Recommendation letters
Letters of recommendation are one of the many benefits of working in a research lab. I will write a letter for any student or lab member who has spent at least one year in the lab. Letters will be provided for shorter-term lab members in exceptional circumstances (e.g., new graduate students or postdocs applying for fellowships). I maintain this policy because I do not think that I can adequately evaluate someone who has been around for less than a year.

To request a letter of recommendation, please adhere to the deadline requirements described above. Send me your current CV and any relevant instructions for the contents of the letter. If you are applying for a grant, send me your specific aims or a short summary of the grant. In some but not all cases, I may ask you to draft a letter, which I will then revise to be consistent with my evaluation. This will ensure that I do not miss any details about your work that you think are relevant to the position you're applying for, and it will also help me complete the letter in a timely fashion.

## Research Drive
Almost all of our data is stored on a **secure UCF server**, the "Research drive". You should have full access to it once the lab managers have completed your orientation and onboarding procedures, and it should appear as the R:/ drive on any of the lab's IT-managed computers. Your personal computers are also capable of accessing this data, so long as you are connected to the `UCF_WPA2` wireless network, or use the [UCF VPN](https://www.cst.ucf.edu/wp-content/uploads/service%20desk/NewVPN_user.pdf) to connect to the university network from home.

### Data organization
Our lab's directory on the research drive has a structure like this:
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
      
I encourage you to become very familiar with the structure of the Research Drive - you will be accessing it quite often.

### Data sharing
Not only is data-sharing the right thing to do, we are actually required to do so for any dataset that was funded by the NIH. We will make these datasets publicly available within a year of publishing the first paper from the dataset. You should also be prepared to share any scripts that you used in your published processing & analysis pipeline. Currently, the best option for sharing smaller datasets seems to be the [Open Science Framework](https://osf.io/), the best option for sharing MRI datasets is [OpenFMRI](https://openfmri.org/), and I don't yet know what is the best option for sharing EEG datasets.
