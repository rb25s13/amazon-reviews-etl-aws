# Alexa, can you handle big data?

	 _____  __    __  _____ 
	/  _  \|  |/\|  |/  ___> 
	|  _  ||        |\___  \ 
	\_/ \_/ \__/\__/ <_____/ 


Create DataFrames to match production-ready tables from two big Amazon customer review datasets.
Analyze whether reviews from Amazon's Vine program are trustworthy.


<ul>
<li><p>Use the furnished schema to create tables in your RDS database.</p>
</li>
<li><p>Create two separate Google Colab notebooks and <strong>extract</strong> any two datasets from the list at <a href="https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt">review dataset</a>, one into each notebook.</p>
<p><strong>Note:</strong> It is possible to ETL both data sources in a single notebook, but due to the large data sizes, it will be easier to work with these S3 data sources in two separate Colab notebooks.</p>
</li>
<li><p>Be sure to handle the header correctly. If you read the file without the header parameter, you may find that the column headers are included in the table rows.</p>
</li>
<li><p>For each notebook (one dataset per notebook), complete the following:</p>
<ul>
<li><p>Count the number of records (rows) in the dataset.</p>
</li>
<li><p><strong>Transform</strong> the dataset to fit the tables in the <a href="../Resources/schema.sql">schema file</a>. Be sure the DataFrames match in data type and in column name.</p>
</li>
<li><p><strong>Load</strong> the DataFrames that correspond to tables into an RDS instance. <strong>Note:</strong> This process can take up to 10 minutes for each. Be sure that everything is correct before uploading.</p>
</li>
</ul>
</li>
</ul>