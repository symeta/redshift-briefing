# redshift-briefing


# 1. Data Migration
- Mysql to Redshift
  * Recommended Way:
    - Mysql Table -(sample cmd shown as below)-> .csv --> S3 -(COPY)-> Redshift
    
    ```sh  
     mysql -B -u username database_name -h mysql_hostname -e "SELECT * FROM table_name;" | sed "s/'/'/;s/t/","/g;s/^/"/;s/$/"/;s/n//g" > table_name_data.csv
    ```

    [COPY](https://docs.aws.amazon.com/redshift/latest/dg/r_COPY.html)


# 2. Data Transfer Leveraging on DX rather than public internet
- [private link]https://docs.aws.amazon.com/AmazonS3/latest/userguide/privatelink-interface-endpoints.html


# 3. Redshift Table Design
- Dist Key
- Sort Key
- Sizing

# 4. Redshift Operation

- WLM
- QMR
- Concurrent-Scaling
- Resizing
- Data Sharing
- Materialized View

# 5. Redshift Performance Optimization
