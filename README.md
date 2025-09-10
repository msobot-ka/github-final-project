Part 1 - GitHub UI
Estimated Time: 30 minutes

Scenario
You recently got hired as a developer in a micro-finance startup with a mission to empower and provide opportunities for low income individuals. The core team currently uses Subversion (SVN) for managing code. They want to slowly move their code to Git. You are asked to host their sample code to calculate simple interest on GitHub in a new repository as the first step in this journey. You will not only host the script, but also follow best practices introduced in this course and create supporting documents for the open source project including a code of conduct, and contribution guidelines. Additionally, the repository should be available to the community under the Apache License 2.0.

Objectives
After completing this lab, you would have demonstrated that you can:

Create a new repository in your GitHub account.
Select the appropriate license for your project.
Create a README.md file that explains the purpose of the project.
Create a Code of Conduct markdown that explains how you want the community to behave and interact with each other.
Create a Contribution Guidelines markdown that tells the community how to contribute.
Commit the new files to the repository.
Note: Throughout this lab, you will be prompted to copy and paste URLs into an editor and save it on your own device. These URLs will be uploaded for peer review in the Final Submission section of the course. You can use any editor app to keep note of your URLs.

Task 1: Create a GitHub repository
Create a new GitHub repository called "github-final-project" and make sure that it is public.

Select the Add a README file and Choose a license check boxes. Pick Apache 2.0 License from the drop down.

Click Create repository. Your repository is created and includes the README and LICENSE files. Now, you are ready to update your repository files to include useful information for your community.

Save the URL of the repository in a Notepad to submit later for peer review.

Task 2: Add a license file
As part of Task 1, you picked a licence when creating the repository.
Open the LICENSE.md file and check that its content are pointing to Apache License 2.0.
Task 3: Update the README file
Add the following information to the file:
1
2
3
4
5
6
7
8
A calculator that calculates simple interest given principal, annual rate of interest and time period in years.
Input:
   p, principal amount
   t, time period in years
   r, annual rate of interest
Output
   simple interest = p*t*r

Copied!

Wrap Toggled!
Optional - You can continue to update the README file as you develop your project. You can find some ideas for useful README content from the following resources:

Github README
Make a README
Awesome README
Task 4: Add a code of conduct
A code of conduct helps set the ground rules for the behavior of your project's participants. It defines standards for how to engage in a community.

GitHub provides templates for common codes of conduct to help you quickly add one to your project. To add a code of conduct to your project, complete the following steps:

Add a new file named CODE_OF_CONDUCT.md to the root folder of the repository with the "Contributor Covenant" template.

Go to your repositories homepage and check if the file has been created.

Task 5: Add contribution guidelines
The contribution guidelines tell project participants how to contribute to the project. To add contributions guidelines, complete the following steps:

Create a new file named CONTRIBUTING.md in the root directory of the repository with the following information:

1
All contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome.

Copied!

Wrap Toggled!
Optionally, you can review the following guides for examples of contribution guidelines and update this file.

Contributing to Legit Info, a Call for Code for Racial Justice Project
Contributing to OpenEEW
Contributing to Atom
How to contribute to Ruby on Rails
Commit the file into the main branch and check if it is listed on the homepage of the repository.
Task 6: Host the script file
Create a new file named simple-interest.sh in the root directory of the repository.

Add the following code in the new file:

1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
   #!/bin/bash
   # This script calculates simple interest given principal,
   # annual rate of interest and time period in years.
   # Do not use this in production. Sample purpose only.
   # Author: Upkar Lidder (IBM)
   # Additional Authors:
   # <your GitHub username>
   # Input:
   # p, principal amount
   # t, time period in years
   # r, annual rate of interest
   # Output:
   # simple interest = p*t*r
   echo "Enter the principal:"
   read p
   echo "Enter rate of interest per year:"
   read r
   echo "Enter time period in years:"
   read t
   s=`expr $p \* $t \* $r / 100`
   echo "The simple interest is: "
   echo $s

Copied!

Wrap Toggled!
Commit the file into the main branch.

