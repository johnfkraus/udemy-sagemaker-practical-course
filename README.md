# udemy-sagemaker-practical-course

Source: 
https://www.udemy.com/course/practical-aws-sagemaker-6-real-world-case-studies/learn/lecture/20041184#questions/12536442


broken udemy sagemaker code:
•	from sagemaker.amazon.amazon_estimator import get_image_uri
•	container = get_image_uri(boto3.Session().region_name, 'linear-learner')
•	try
•	from sagemaker.image_uris import retrieve
•	container = retrieve('linear-learner', boto3.Session().region_name)

•	@Aruun I am making changes throughout the entire course for deprecated methods from the SageMaker Python SDK v2.x. THANK YOU for pointing these out and bringing it to my attention. There are more than the ones you have pointed out. I advise going through and "redownloading" the Juypter notebooks that have been updated.
•	I have pushed all of the changes. These includes:
•	Deprecated get_image_uri which is now image_uri.retrieve
•	Renaming training_instance_count to instance_cout
•	Renaming training_instance_type to instance_type
•	Deprecated s3_input which is now sagemaker.inputs.TrainingInput
•	Renamed csv_serializer and json_deserializer to sagemaker.serializers.CSVSerializer() and sagemaker.deserializers.JSONDeserializer() respectively
•	Please see the changes in the commit here: https://github.com/ACloudGuru-Resources/Course_AWS_Certified_Machine_Learning/commit/ab99654f4c7150a3f8d18b9e35b9d1f696707448


