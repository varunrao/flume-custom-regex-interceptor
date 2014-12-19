flume-custom-regex-interceptor
==============================
Simple interceptor which is a extension to the Flume regex filter interceptor.
The use can specify a list of fields that needs to be pulled out of the event bosy to be sent to the Channel/Sink

Added a new filed called indexSelector
agent.sourcs.agent_name.interceptors.filter_name.regex=INFO(.*)Python(.*)Test(.*)
agent.sourcs.agent_name.interceptors.filter_name.indexSelector=1,2

1,2 will pull the first 2 fields of the regular expression matching string.
