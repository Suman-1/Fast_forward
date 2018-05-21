Hello here i am updating readme with new information 

##### UNDOING THE CHANGES IN THE WORKING DIRECTORY #####


   


This is the magic thing you can do in it 

You accidently deleted a file OR updated a file  in the git and 

later you noticed that the file you deleted is not as 

according to your choice

YOu can also undo the changes you made 

By simply using the command 

There are two options for that 

You can do either checkout or hard reset 

----checkout favours for modification 
-----Hard reset favours for both 

=====>>> Checkout   #git checkout <file-name-that-you-want-to-undo-the-changes>


======>>>>> #git reset --hard 


This is the magic that you can do with the git but this only works before commit 





	###### UNDOING AND REDOING CHANGES TO THE REPOSITORY #####

When you do above commands only the working directory changes that the log remains the same 
For that you have do to simply is 

 	#git reset --soft HEAD~1 (Move 1 step back)
		It takes the last commit from the repository 

	#git  reset --hard HEAD~1
		it will delete the last commit and discard all the changes




	#####CLEANING THE WORKING COPY ###

	IF there is the stray files in your directory which you don't need then you can remove the stray file easily 


	Command to remove the stray file
		#git clean -n (tells that what will happen)
		
		#git clean -f (Removes the files makes working directory clean by removing unnecessary files that you
				didn't commited)

	

	### IGNORING THE FILES WITH .gitignore ###
		This is the way that tells that you don't want to add the file in the repos
		this method works as the type that you created a file that you don't want to 
		commit it 
		For example:		
			You Created a file (mkdir log ) and in the log dir you added (touch log.txt)
			and then we know that log changes frequently 
			in this condition what you can do is simply ignoring the log dir by specifying in the 
			.gitignore (vim .gitignore) and put the file system there

			In my case, i have a log dir 
					what i can do simply is==>>> log/
					other ways are /log ===>>>Root of the repo anything in the log dir
					/log/*.txt ====>>Only the .txt is ignored of that dir
					/log/*.log ===>>> Only the .log is ignored of that dir 
