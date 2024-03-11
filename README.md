# redshift-briefing

# A Recommended Architecture Diagram 

<img width="492" alt="image" src="https://github.com/symeta/redshift-briefing/assets/97269758/b6071d85-94f3-4cc2-8f81-b0e188018ec0">


- key points:
  * it's better that mysql instance, redshift cluster, and sagemaker notebook instance in the same vpc.
 
- guidance resource:
  * [Incremental Data Load from RDS MySQL to Redshift via Glue](https://www.youtube.com/watch?v=R-1go56ip5g)
  * [Sagemaker Notebook Jupyter work with Redshift](https://github.com/aws-samples/amazon-redshift-commands-using-sagemaker/blob/master/sagemaker_redshift.ipynb)
  * [Amazon Managed Workflow for Apache Airflow](https://docs.aws.amazon.com/mwaa/latest/userguide/what-is-mwaa.html)
  * [Glue CLI](https://docs.aws.amazon.com/cli/latest/reference/glue/)

- sizing
  * [compute capacity](https://docs.aws.amazon.com/redshift/latest/mgmt/serverless-capacity.html)
  * [configure compare](https://github.com/aws-samples/amazon-redshift-config-compare)

- think forward
  * [RDS for Mysql zero-etl Integration with Redshift](https://aws.amazon.com/about-aws/whats-new/2023/11/amazon-rds-mysql-zero-etl-integration-amazon-redshift-public-preview/)
