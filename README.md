# KotlinConf23-dataframe
Jupyter notebooks and data from my talk at KotlinConf '23, "*Replacing SQL with Kotlin `dataframe` on the Las Vegas Strip*" ([YouTube](https://www.youtube.com/watch?v=sDZWiu9nnuU&list=PLlFc5cFwUnmwcJ7ZXyMmS70A9QFyUu1HI), [slides](https://cfnine.com/kc23))

## files
- [KotlinConf_FollowUp.ipynb](/KotlinConf_FollowUp.ipynb) : updated Jupyter notebook, with SQL equivalents
- [KotlinDataframeDemo.ipynb](/KotlinDataframeDemo.ipynb) : original Jupyter notebook used during presentation
- [KotlinConf_sampledata.zip](/KotlinConf_sampledata.zip) : sample data for running the notebook, as CSV files
- [KotlinExampleDDL.sql](/KotlinExampleDDL.sql) : sample data as a series of DDL statements (CREATE TABLE, INSERT INTO, etc)

## update 2023-05-28
Some feedback indicated interest in direct SQL-to-dataframe translation examples. I've created a [follow-up Jupyter notebook](/KotlinConf_FollowUp.ipynb) which interlaces the Kotlin dataframe code with the equivalent SQL, using SQL Server's T-SQL syntax. You'll note the SQL gets longer and longer each time. Further, there's a lot of use of the T-SQL PIVOT function which is not universal and may not translate to other databases. Most of the SQL can be run at [SQL Fiddle](http://sqlfiddle.com/#!18/e2e99/1/0) if you don't have SQL Server. "Most," because SQL Fiddle has a character limit, and including the `players` table would exceed that limit. Everything before that is replicable.

## setup
Remember, this is a Jupyter notebook file using the Kotlin kernel, which needs you'll need 
- Python
- Jupyter ([instructions here](https://jupyter.org/install))
- Kotlin kernel ([instructions here](https://github.com/Kotlin/kotlin-jupyter))

Once you have Jupyter running, you can open one of the notebook (.ipynb) files above. You'll likely have to edit some file paths to access the data files after you download and extract them on your system.

## need help?
Please feel free to reach out! Whether you saw the presentation live or on YouTube, if you have any questions I'm happy to try to help. I recognize trying to simulate an entire database marketing process in about 12 minutes (even a simplified one) is hard to follow and many details and explanantion was left out... so please ask any questions. andy [at] cfnine [dot] com

## KotlinConf
Thanks again to the KotlinConf team for the opportunity to present. Don't forget to watch all the other [terrific KotlinConf presentations](https://kotlinconf.com/talks). 

