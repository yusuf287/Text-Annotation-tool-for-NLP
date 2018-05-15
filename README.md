# Text-Annotation-tool-for-NLP
Getting the annotated data to train model to perform Natural Language Processing task is one of the most tiring and boring work. This tool has been created to ease that process. There are two versions of it. One where tkinter is used to build GUI for the tool and other is just a CLI.

This tools is specifically for Resume annotation. But it can always be changed to other domains as required.You just need to go and change the labels.
The plan is to annotate each individual line in two different classes i.e. Line Type and Line Label. Line Type will give us the detail about the priority of data like whether it is header or meta-data(title) or only content (description about the title). Line Label categorizes the lines into different segments like Education, Skill set, Experience etc. This list will be saved as python dictionary in python and numbers will be used as keys as described below. This dictionary will be used wherever the reference is required to make everything in sync.

If any change is required in line classification, the direct change to this list will work. Please find below the description of each type and labels.

line_types =

{0:'header', 1:'title', 2:'content'}
line_labels =

{0:'experience', 1:'skillset', 2: 'education', 3:'personal', 4:‘miscellaneous'}
Line Types:

•	Header (0): It is the title line which defines the beginning of any new section for. eg. "Experience", "Education", "Personal" etc.
•	Title (1): It is the sub-title which defines the sub-categories in sections, if any. For eg. "Research Assistant" could be the sub-title in "Education", "Sales Executive" could be the sub-title in "Experience" etc.
•	Content (2): This line will contain all the description about the particular segment.

Line Labels:

•	Experience (0): It includes all the line describing any kind of experience.
•	Skillset (1): It includes all the technical or domain specific skills.
•	Education (2): It includes details about the educational background of candidate like year of passing, name of university, course etc.
•	Personal (3): It will contain all the information about the candidate including their email-id, social networking address like LinkedIn, GitHub profiles etc.
•	Miscellaneous (4): It will contain any other details which is not described in the above the labels.
