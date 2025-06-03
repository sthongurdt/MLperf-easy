# Extracting Results.

Extracting the results is simple. When you run oar_exec.sh, two files are created in the cluster directories you use. You must verify that the cluster directories exist.
Inside the cluster directory, you will find two files named `OAR_%job_id%_framework_model.err` and `OAR_%job_id%_framework_model.out`.

To download the metrics, we'll follow these steps: download the job_id metrics and start processing them. Copy the job_ids of the tests I perform to download the metrics. From the mlperf directory, enter the result directory (create it if it doesn't exist).
```
mlperf$ cd result
```
To download the metrics we will use the command recommended by the documentation.
```
curl 'https://api.grid5000.fr/stable/sites/lyon/metrics?job_id=job_id' >> job_id_framework_model
```
