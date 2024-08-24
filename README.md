
Install spark
https://github.com/DataTalksClub/data-engineering-zoomcamp/blob/main/05-batch/setup/linux.md

```bash
export SPARK_HOME="${HOME}/spark/spark-3.3.2-bin-hadoop3"
export PATH="${SPARK_HOME}/bin:${PATH}"
```

## Use pyspark
Check the py4j version:
```bash
ls ${SPARK_HOME}/python/

# creante environment
export PYTHONPATH="${SPARK_HOME}/python/:$PYTHONPATH"
export PYTHONPATH="${SPARK_HOME}/python/lib/py4j-0.10.9-src.zip:$PYTHONPATH"

jupyter notebok
```

## Run spark
```bash
 spark-shell
```

### hvfhs structure

```bash
types.StructType([    
    types.StructField('hvfhs_license_num', types.StringType(), True), 
    types.StructField('dispatching_base_num', types.StringType(), True), 
    types.StructField('pickup_datetime', types.TimestampType(), True), 
    types.StructField('dropoff_datetime', types.TimestampType(), True), 
    types.StructField('PULocationID', types.IntegerType(), True), 
    types.StructField('DOLocationID', types.IntegerType(), True), 
    types.StructField('SR_Flag', types.StringType(), True)
])
```