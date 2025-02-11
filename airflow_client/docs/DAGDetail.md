# DAGDetail

DAG details.  For details see: [airflow.models.DAG](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/models/index.html#airflow.models.DAG) 

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dag_id** | **str** | The ID of the DAG. | [optional] [readonly] 
**root_dag_id** | **str, none_type** | If the DAG is SubDAG then it is the top level DAG identifier. Otherwise, null. | [optional] [readonly] 
**is_paused** | **bool, none_type** | Whether the DAG is paused. | [optional] 
**is_active** | **bool, none_type** | Whether the DAG is currently seen by the scheduler(s).  *New in version 2.1.1*  *Changed in version 2.2.0*&amp;#58; Field is read-only.  | [optional] [readonly] 
**is_subdag** | **bool** | Whether the DAG is SubDAG. | [optional] [readonly] 
**last_parsed_time** | **datetime, none_type** | The last time the DAG was parsed.  *New in version 2.3.0*  | [optional] [readonly] 
**last_pickled** | **datetime, none_type** | The last time the DAG was pickled.  *New in version 2.3.0*  | [optional] [readonly] 
**last_expired** | **datetime, none_type** | Time when the DAG last received a refresh signal (e.g. the DAG&#39;s \&quot;refresh\&quot; button was clicked in the web UI)  *New in version 2.3.0*  | [optional] [readonly] 
**scheduler_lock** | **bool, none_type** | Whether (one of) the scheduler is scheduling this DAG at the moment  *New in version 2.3.0*  | [optional] [readonly] 
**pickle_id** | **str, none_type** | Foreign key to the latest pickle_id  *New in version 2.3.0*  | [optional] [readonly] 
**default_view** | **str** |  | [optional] [readonly] 
**fileloc** | **str** | The absolute path to the file. | [optional] [readonly] 
**file_token** | **str** | The key containing the encrypted path to the file. Encryption and decryption take place only on the server. This prevents the client from reading an non-DAG file. This also ensures API extensibility, because the format of encrypted data may change.  | [optional] [readonly] 
**owners** | **[str]** |  | [optional] [readonly] 
**description** | **str, none_type** | User-provided DAG description, which can consist of several sentences or paragraphs that describe DAG contents.  | [optional] [readonly] 
**schedule_interval** | [**ScheduleInterval**](ScheduleInterval.md) |  | [optional] 
**timetable_description** | **str, none_type** | Timetable/Schedule Interval description.  *New in version 2.3.0*  | [optional] [readonly] 
**tags** | [**[Tag], none_type**](Tag.md) | List of tags. | [optional] [readonly] 
**max_active_tasks** | **int, none_type** | Maximum number of active tasks that can be run on the DAG  *New in version 2.3.0*  | [optional] [readonly] 
**max_active_runs** | **int, none_type** | Maximum number of active DAG runs for the DAG  *New in version 2.3.0*  | [optional] [readonly] 
**has_task_concurrency_limits** | **bool, none_type** | Whether the DAG has task concurrency limits  *New in version 2.3.0*  | [optional] [readonly] 
**has_import_errors** | **bool, none_type** | Whether the DAG has import errors  *New in version 2.3.0*  | [optional] [readonly] 
**next_dagrun** | **datetime, none_type** | The logical date of the next dag run.  *New in version 2.3.0*  | [optional] [readonly] 
**next_dagrun_data_interval_start** | **datetime, none_type** | The start of the interval of the next dag run.  *New in version 2.3.0*  | [optional] [readonly] 
**next_dagrun_data_interval_end** | **datetime, none_type** | The end of the interval of the next dag run.  *New in version 2.3.0*  | [optional] [readonly] 
**next_dagrun_create_after** | **datetime, none_type** | Earliest time at which this &#x60;&#x60;next_dagrun&#x60;&#x60; can be created.  *New in version 2.3.0*  | [optional] [readonly] 
**timezone** | **str** |  | [optional] 
**catchup** | **bool** |  | [optional] [readonly] 
**orientation** | **str** |  | [optional] [readonly] 
**concurrency** | **float** |  | [optional] [readonly] 
**start_date** | **datetime, none_type** | The DAG&#39;s start date.  *Changed in version 2.0.1*&amp;#58; Field becomes nullable.  | [optional] [readonly] 
**dag_run_timeout** | [**TimeDelta**](TimeDelta.md) |  | [optional] 
**doc_md** | **str, none_type** |  | [optional] [readonly] 
**params** | **{str: (bool, date, datetime, dict, float, int, list, str, none_type)}** | User-specified DAG params.  *New in version 2.0.1*  | [optional] [readonly] 
**end_date** | **datetime, none_type** | The DAG&#39;s end date.  *New in version 2.3.0*.  | [optional] [readonly] 
**is_paused_upon_creation** | **bool, none_type** | Whether the DAG is paused upon creation.  *New in version 2.3.0*  | [optional] [readonly] 
**last_parsed** | **datetime, none_type** | The last time the DAG was parsed.  *New in version 2.3.0*  | [optional] [readonly] 
**template_search_path** | **[str], none_type** | The template search path.  *New in version 2.3.0*  | [optional] 
**render_template_as_native_obj** | **bool, none_type** | Whether to render templates as native Python objects.  *New in version 2.3.0*  | [optional] [readonly] 
**any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


