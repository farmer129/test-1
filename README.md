# README

Before you make any difference to the repo, please check STEP and CAUTION below!!!
 
# STEP

## If you are adding/uploading some files onto the site on github, please follow the step below.  
1. Check your file, and it should be PDF type and at most 30 pages. The category and created data will be named according to the name of PDF.  
2. Find the script.py in the base path of the repo, and check the content from line-14 to line-36.  
3. Follw the comments, if the values are not correct, please adjust them manually.  
4. Fine and open the 'Source' dirctory in the  base path of the repo, and upload your file into the dirctory.  
5. Wait for a while and everything will be done automatically.  
6. You can check the github actions (click 'actions' above the repo and below the repo name). Please do not make any change before all actions finish.  
7. After all actions are done, you can check the created data files in '_datasets', and all created data files will name like 'PDFName-1.md', you can change it directly as you like, but please don't change the file type.  

## If you are adding/uploading some files onto the site on local device, please follow the step below. 
1-3. Same as the step 1 above.  
4. Please paste your PDF file in the Source directory.  
5. Then use git add/ git commit/git push(to the main branch) to make difference.  
6-7. Same as the step 1 above. 

# CAUTION
## Before you make difference, please check cautions below if you are not familiar with them.
1. Only PDF file can be accepted.  
2. To make the system work well, only 30 pages can be processed within 24 hours. If your file includes more than 30 pages, only the first 30 pages will be processed. If there are multiple PDFs are uploaded together, the total pages can not exceed 30.   
3. Your PDF will be deleted after the process done automatically to keep the source dirctory clear.  
4. The time of processing is according to how many pages in the PDF, generally 50 seconds for each page.  
5. Only main branch will call the github actions, so any change in sub-branch won't make difference to the site.  

# For administrator (the repo owner)
## Manage the repo and site
1. Upload files: the ways introduced above are suitable for both administrator and collaborators.  
2. Delete/Edit files: Go to the '_dataset' directory, then find and delete/edit the files you want directly.  
3. Delete/Edit categories: Go to the '_data' directory and fine 'categories.yml', then you can delete or hide categories as you want.  
4. Add organizations: Find the '_organizations' directory and create one .md type file as the form of existed file.  
## Give permission
### If you want to give others permission to contribute the repo. Please follow the step below.
1. Go to 'Setting' --> 'Collaborators' --> Check your account --> 'Manage access' Add people. Invite your collaborators into the repo. Then they could make changes.  
2. 'Setting' --> 'Actions' --> 'General' --> 'Workflow permissions'. Switch to 'Read and write permission' from 'Read repository contents and packages permissions'.

# Q&A
#### Q: When I upload a file and fail with 'that’s a big file. Try again with a file smaller than 25MB.  
A: Because github doesn't allow user to upload a file bigger than 25MB directly on github site. You can try to clone the repo to you local repo and move your PDF into the directory 'Source' and push it onto remote repo. If your PDF is larger than 100MB, please use Git LFS (Large File Storage).
#### Q: The github actions fail, the error is nothing to commit.
A: This situation always happen when you make changes but not upload file in 'Source' directory. Take it easy, it won't lead to any crash or unexpected.
#### Q: I upload a PDF file but no content in the result (created files).
A: It may happen if the system has processed more than 30 pages within 24 hours. When a same IP uses Trancribus frequently in a period, it will always receive a ban (last for 24 hours) from Transcribus. If so, please try your work after the ban, and notice that the existed files in '_dataset' may need to be deleted manually.
# Any other IT question:
#### Please contact team Charlie
#### Frank Chen (z.chen5.21@abdn.ac.uk / frankchen2202@163.com)
