For replication the demo assets in your RACE environment, perform the following steps. 

* Book the latest EEC171 image.

#### There are 3 models used 

* Fixed Premium Prediction Model
	* To replicate this model, download "Fixed Premium Prediction.txt" - XML for Fixed Premium Models.
	* Import the XML in your enviroment. 
	* Import the "underwriting_data.csv" from /datasets folder.

* Flexi Premium Prediction Model
	* Open Model Studio and import the "Flexi Rate Model.zip"
	* Import "flexi_data_latest.csv" from /datasets folder
	* Run the pipeline

* Add on Prediction Prediction Model
	* Open Model Studio and import the "Flexi Rate Model.zip"
	* Import "final_add_on_data.csv" from /datasets folder
	* Run the pipeline


* We also have create a Python Xsell model, the details can be found in "python_XSELL_model.ipynb". Refer the steps documented in the jupyter notebook to create and operationalize your model. 