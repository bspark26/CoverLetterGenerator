# CoverLetterGenerator

I created this powershell script because I was tired of manually editing a few words of my Cover Letter when applying to jobs.

It works like this: 

Take for example my cover letter, I was tired of going through my CV and changing the Role, Company Name, and Soft Skills related to the position.
I replaced thoes 3 items with Placeholders eg: (Position_Name) instead of 'Junior Developer'.

It takes a word document **must be a .docx file** and uses it as a template.

The script is only programmed to find the 3 specific placeholder values I set in my document as they wont change.

Set your path in the $template line to your document you wish to template, you can add as many placeholders as you want you just need to add in the $variable = Read-Host -Prompt 'insert prompt string here'

Add or change the variable targets '$body = $body.Replace("(Position_Name)", $Position_Name )' to match your set place holders.

What i like most is that the script will output a new file with the same name except it appends '-current.docx' to the end of the file.
Each time you run the script the output document is over written so you wont have a build up of files.

I plan to grow this a bit over the next while, maybe make a basic GUI app in .net MVC and change the hard coded file path to a file dialog selection.
