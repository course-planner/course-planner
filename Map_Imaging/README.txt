Run Map_Image.py:

	python Map_Image.py


Crop Map Images (In Mac OS):
	
	1) Open an image generated from the Map_Image.py script in Photoshop
	2) In Photoshop, record a custom action (Window -> Action -> Record)
		2a) Image -> Canvas Size (Width: 11, Height: 9) -> OK
		2b) Image -> Image Size (Width: 5.5, Height: 4.5) -> OK 
		2c) File -> Save As... -> (Navigate to Map_Crops), (Format is PNG, save as a copy) -> Save
		2d) Close the working image (NOT THE WINDOW)
	3) Click “stop” to stop recording action, and save as “Map_Crop”
	4) Navigate to Map_Crops in Finder, delete the newly created image
	5) Return to Photoshop, in an empty file
	6) File -> Automate -> Batch
		6a) Set: Default Actions
		6b) Action: Map_Crop
		6c) Source: Navigate to Map_Images folder
		6d) Select: Suppress File Open Options Dialogs
		6e) Destination: None
		6f) Click OK to start Batch process
	7) Once Batch process is complete, navigate to Map_Crops folder
		7a) Select all images -> Right Click -> Rename ___ items
		7b) Replace Text -> Find: “ copy” (Space needs to be included) -> Replace With: “” (Nothing) -> Rename