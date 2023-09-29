# Resume_data_finetuning_on_GPT-3.5.
Instructions on how to run your code.
here's a structured text explanation with execution commands for the provided Python code snippets:

Step 1: Parsing Resumes
To parse resumes located in a specified folder and extract relevant data, use the following code snippet:
Execute the parsing resumes function with the resume folder path
resume_folder = "/path/to/resume/folder"
parsed_data = parse_resumes(resume_folder)

Step 2: Generating Resume Summaries
To generate a summary for a specific resume by providing its resume ID, utilize the following code 
snippet:
Execute the getResumeSummaryById function with the desired resume ID
resume_id = "1"  # Replace with the desired resume ID
summary = getResumeSummaryById(resume_id)

Step 3: Finding Similar Resumes
To find resumes similar to a target resume based on content comparison, execute the following code:
Define the target resume ID
target_resume_id = "1” # Replace with the ID of the target resume
Execute the getSimilarResume function with the target resume ID and parsed data
result = getSimilarResume(target_resume_id, parsed_data)

Step 4: Searching for Resumes by Skills
To search for resumes that match specific skills, run the following code:
Define the target skills to search for
target_skills = ["Software developer", "Java Developer"]  # Use the skills you want to search for
Execute the get_Resume_byskill function with the target skills and parsed data
result = get_Resume_byskill(target_skills, parsed_data)
These execution commands correspond to the respective code snippets and perform tasks such as parsing resumes, generating summaries, finding similar resumes, and searching for resumes by skills


Assumption: -
During the challenge, I made the following assumption and decisions:
Assumption: I assumed that all the keys, namely "name," "Title/Role," "Skills," "Technical Skills," "experience," and "background," are already available in the given resumes.
Justification: By assuming the presence of these keys, I could design and implement the code more efficiently to parse and extract data from the resumes accurately. This assumption streamlined the development process and aligned with the context of the challenge, where the focus was primarily on demonstrating the ability to work with resume data and utilize AI models for tasks like summarization and comparison.
In real-world scenarios, resume data can vary significantly in structure and content. In practice, handling missing or inconsistent data would require additional data preprocessing and error handling techniques. However, for the purpose of this challenge, assuming the presence of these keys allowed for a more straightforward and focused implementation of the provided tasks.
