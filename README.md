# **BOTTOM LINE UP FRONT:**
This custom-built program automates a series of button-presses (between X and Y) down to Z, using .csvs in Excel along with Selenium and Chromedriver to send emails, record activity, schedule to-do's, and change statuses accordingly.


# **BACKGROUND**
Job: academic recruiter. This program cuts down dramatically on the time and energy costs of working this job.

The core purpose of this job is to enroll students, thus making money for the university.

Because this job involves a great deal of reaching out to unresponsive leads, the note-taking efforts involved in tracking those leads consumes a great deal of time, even as it takes a very repetitive and monotonous shape.

I learned in school to recognize time-consuming, monotonous labor as something that could be automated away. So I developed code that saves energy and time in 2 ways:
(1) Almost all labor is done in an excel sheet, cutting down on the need to wait for .html pages to load.
(2) Monotonous series of button-presses are executed with single button-presses housed inside of the Python code.


# **LABOR AND CODE IN ACTION**
In the case of an unresponsive lead, there are 4 small tasks to take care of:
(1) Email the lead (i.e. "we saw you were interested in our program; when would you like to talk?" etc.)
(2) Log your activity
(3) Create your next "to-do"
(4) Change the lead's status if necessary ("qualified", "applied", "Do Not Call", etc.)

Each task above is automated by my code. In its current iteration (11-12-13), there are 8 cells which determine the execution of these tasks. Because labor can be executed inside of the excel file, I often copy and paste the same 8 cells for an entire days' worth of unresponsive leads, rendering the required button-presses as follows:
1. CTRL+C
2. DOWN ARROW
3. CTRL+V

In the event that a lead IS responsive, I do need to enter custom values for these 8 cells as required. But the low volume of responsive leads and high volume of personalized labor required to serve them makes attempts to cut down any further on time/energy impractical.

When an entire sheet full of leads has been processed, I save it to a .csv file. My Python code reads the .csv file and uses Selenium and Chromedriver to send emails, record activity, schedule to-do's, and change statuses accordingly.

# **OUTCOME**
The end result is much less time spent on unresponsive leads, freeing up much more time to devote to responsive ones.