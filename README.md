# NicheMapper
This is only for demonstration and practice shared within Williams lab. Please don't use it for any purpose of research, publications, or other public use.


HOW TO GET ACCESS TO NICHE MAPPER:
Niche Mapper is a program to simulate individual animal (birds and mammals, currently) behaviors dynamically under certain environmental conditions. The program is run only in Windows system currently. Please make sure that you run the program in Windows systems. 
•	Download from Williams lab server:
o	(You have to use VPN or work with lab computer in order to get access to Williams lab server. The way to use VPN to access Williams lab server is in lab wiki: http://geography.wisc.edu/wlabwiki/doku.php/lab_info/access_server.)
o	path: Williams\Lab_Climate_Data\LabPractice\NicheMapper
	
•	Download from Github:
o	(You have to install Github first. The way to install and use Github is in Scott’s blog: http://scottsfarley93.github.io/tutorial/2016/09/10/Williams-Lab-Github-Lesson.html)
1)	log into your Github account;
2)	import repository from WilliamsPaleoLab/NicheMapper:
a.	click the plus sign on the upper right corner;
b.	choose “import repository”;
c.	copy the cloned URL: https://github.com/WilliamsPaleoLab/NicheMapper.git;
d.	create your own repository where you want to play the Niche Mapper, for example, NicheMapper_Practice;
e.	click the button “Begin import” on the lower right corner; it may take one minute to import the Niche Mapper repository, feel free to close the window if you think there are too many open windows and you feel too crowded;
f.	now you have the Niche Mapper repository in your Github. Have fun to play with Niche Mapper!


HOW TO USE NICHE MAPPER:
The input files in the Niche Mapper, including physical/biological traits of animal and environmental conditions, are listed as below: 
•	alomvars.dat: body and fur characteristics of the animal, variables are explained in “Alomvars input file notes.docx”;
•	endo.dat: biophysical characteristics of the animal, including metabolic rate, weight, fat mass percentage, etc., variables are explained in “Endo input file notes.docx”;
•	micro.dat: environmental conditions that animal live in, including monthly min/max average temperature/relative humidity/cloud coverage/wind speed, etc..
•	DIVETABL.DAT: diving traits of the animal, if the animal can dive and the diving option is checked in endo.dat.
•	solar.dat: solar radiation characteristics. For the current version, it cannot be changed.
•	dataky.dat: input file help to run the program month by month. It cannot be changed.
The steps to run Niche Mapper program are listed as below:
1)	set variables in the input file, including alomvars.dat, endo.dat, and micro.dat; DIVETABL.DAT is set as an option if the animal can dive;
2)	run Micr2010a.exe. The environmental conditions are analyzed now and several files about environmental conditions are produced;
3)	run Endo2013b.exe. The individual animal behaviors are analyzed now and the hour/month/year behavior characteristics are produced in excel files, as set in endo.dat;
4)	the variables in hour/month/year excel files are explained in “Output Explanation.doc”.


HOW TO RECORD YOUR CHANGES IN GITHUB:
Some tips to help run Niche Mapper using Github:
•	open terminal;
•	set the local directory where you want the Niche Mapper cloned, for example, the desktop: cd Desktop;
•	clone the Niche Mapper repository to your local directory: git clone <your Niche Mapper repository web URL> (get the URL by click the button “Clone or download” on the upper right corner on the page of your Niche Mapper repository);
•	set to the directory of Niche Mapper: cd <your local directory>, for example, cd NicheMapper_Practice;
•	play with Niche Mapper program;
•	record the changes in the folder:
o	git add .;
o	git commit –m “<the changes you made>”;
•	push back to the repository: git push origin master.


PRACTICE DEMO
•	Woolly mammoth cannot survive under Madison temperature. How about Alaska temperature? Change the temperature to Praetorius 2015 temperature, which is in “climate_month.csv”;
•	Yue thinks woolly mammoth is 3 m tall, but Jack disagrees and thinks they should be taller. Let’s increase the size of woolly mammoth from 300 cm to 400 cm to see what can happen;
•	The hair density of woolly mammoth is tricky. Try 0.15, 2, and 20 hair/cm2 to see what will happen to metabolism;
•	The water percentage in the dung… Let’s try 0.15, 0.50, and 0.80;
•	Currently the woolly mammoth has no way to cool down, and that’s, perhaps, why they cannot survive under warmer climate. Try diving? I tried one successfully, but failed later many times for unknown reasons… 
