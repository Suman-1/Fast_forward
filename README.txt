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
