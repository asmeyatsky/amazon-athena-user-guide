# Running SQL Queries Using Amazon Athena<a name="querying-athena-tables"></a>

You can run SQL queries using Amazon Athena on data sources that are registered with the AWS Glue Data Catalog and data sources that you connect to using Athena query federation \(preview\), such as Hive metastores and Amazon DocumentDB instances\. For more information about working with data sources, see [Connecting to Data Sources](work-with-data-stores.md)\. When you run a Data Definition Language \(DDL\) query that modifies schema, Athena writes the metadata to the metastore associated with the data source\. In addition, some queries, such as `CREATE TABLE AS` and `INSERT INTO` can write records to the dataset—for example, adding a CSV record to an Amazon S3 location\. When you run a query, Athena saves the results of a query in a query result location that you specify\. This allows you to view query history and to download and view query results sets\.

This section provides guidance for running Athena queries on common data sources and data types using a variety of SQL statements\. General guidance is provided for working with common structures and operators—for example, working with arrays, concatenating, filtering, flattening, and sorting\. Other examples include queries for data in tables with nested structures and maps, tables based on JSON\-encoded datasets, and datasets associated with AWS services such as AWS CloudTrail logs and Amazon EMR logs\.

**Topics**
+ [Query Results and Query History](querying.md)
+ [Working with Views](views.md)
+ [Creating a Table from Query Results \(CTAS\)](ctas.md)
+ [Handling Schema Updates](handling-schema-updates-chapter.md)
+ [Querying Arrays](querying-arrays.md)
+ [Querying JSON](querying-JSON.md)
+ [Querying Geospatial Data](querying-geospatial-data.md)
+ [Using ML with Athena \(Preview\)](querying-mlmodel.md)
+ [Querying with UDFs \(Preview\)](querying-udf.md)
+ [Querying AWS Service Logs](querying-AWS-service-logs.md)
+ [Querying AWS Glue Data Catalog](querying-glue-catalog.md)