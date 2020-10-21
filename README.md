# GPoID
Gradual Pattern over Imprecise Data

		 ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━	
				README


			Michaël Chirmeni Boujike
		 ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━


==========================================================================
			Fichiers
==========================================================================
		1.	GPoID-AprioriTID.jar	
		2.	GPoID.R
		3.	test3.data

==========================================================================
			Description des fichiers
==========================================================================
		1.	"GRAPGT-AprioriTID.jar" : librairie Java de l'algorithme AprioriTID modifié;	
		2.	"GRAPGT.R" : approche modifié de modified approach of the T-GPatterns prenant e compte le seuil graduel;
		3.	"test3.data" : dataset; 

==========================================================================
		Exécution (WINDOWS)
==========================================================================	
		1.	Installer R (dernière version 3.6.x);
		2.	Mettre le bin de R dans la variable d'environnement (ex : C:\Program Files\R\R-3.6.0\bin);
		3.	Après installation de R, importer/installer la librairie de Java dans R:
			-	install.packages("rJava")
			-	si la JDK n'est pas installée:
				*	télécharger et installer la jdk (dernière version) : https://www3.ntu.edu.sg/home/ehchua/programming/howto/JDK_Howto.html
				*	créer la variable d'environnement JAVA_HOME and et mettre le chemin de la JDK (ex: JAVA_HOME ="C:\Program Files\Java\jdk1.8.0_171")
		4.	Aller à l'invite de commande, puis dans le dossier contenant le code source et saisissez la commande :
			- "PATH\Rscript" <<File_R>> <<minSupp>> <<minimum_size_of_gradual_pattern>> <<dataset>> <<output_file>> <<K1>> <<K2>> <<column_separator_in_the_dataset>>
			- where K1 and K2 are constants
		   Example :
				- 	Rscript GRAPGT.R 0.08 2 test3.data output.csv 1 0  sd " "
				
==========================================================================
		Exécution (LINUX)
==========================================================================	
		1.	Installer R (dernière version 3.6.x);
		2.	Après installation de R, importer/installer la librairie de Java dans R:
			-	install.packages("rJava")
			-	si la JDK n'est pas installée:
				*	télécharger et installer la jdk (dernière version) : https://www3.ntu.edu.sg/home/ehchua/programming/howto/JDK_Howto.html
				*	créer la variable d'environnement JAVA_HOME and et mettre le chemin de la JDK
		3.	Aller à l'invite de commande, puis dans le dossier contenant le code source et saisissez la commande :
			- "PATH\Rscript" <<File_R>> <<minSupp>> <<minimum_size_of_gradual_pattern>> <<dataset>> <<output_file>> <<K1>> <<K2>> <<column_separator_in_the_dataset>>
			- where K1 and K2 are constants
		   Example :
				- 	Rscript GRAPGT.R 0.08 2 test3.data output.csv 1 0  sd " "
