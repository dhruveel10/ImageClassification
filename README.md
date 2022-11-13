# ImageClassification
The model uses SVM, Random Forest and Linear Regression to classify pictures of different sports personality. The datasets has 7 different players. Chrome extension Fatkun is used to download the images. 
CV2 is used to identify facial characteristics. Images are cropped and stored in a separate folder(folders created dynamically using python os module) such that if the player's eyes are clearly visible, use that image for the dataset else ignore.
Wavelet is used to extract face features of the cropped images and use them to train the dataset.

Result after using GridSearchCV:

	svm	                0.8181818181818182	{'svc__C': 1, 'svc__kernel': 'linear'}
	random_forest	        0.5818181818181818	{'randomforestclassifier__n_estimators': 10}
	logistic_regression	0.8545454545454545	{'logisticregression__C': 1}
