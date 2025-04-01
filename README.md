# interview_MM_DD

Context:
Build Scalable Real-time Application to ingest events/data coming from any mesaging queue and writing it to a object store.

Requirements:

Payload of event in a message queue should be stored to an object store.
In case of any failure of message processing, there should be a auto retry for 2 times.
If message processing fails after all retries, send it to DLQ and process next message.

NFR:
Scale app to consume 100 events/sec
Add a high level design doc in read me for the solution
Implement parallelism in event processing

Validation:
Validate that the event is having a payload attached. If not send it to DLQ.


Infra:

Use any message queue for you choice or familarity. You can get the broker running as a docker instance in you local setup.
Runs the listener apps locally
You can use any object store of your choice. Use your personal account for setting up this store. If having issues, write to a local file.
