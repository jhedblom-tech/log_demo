# log_demo
home assignment

EXPLANATION:

The solution simulates a complete log flow using three small Python scripts.

log_sender.py reads each line from logs.txt and sends it over UDP to a custom syslog port on the server.

syslog_server.py receives the logs, saves it in a date- and source-IP–based folder structure, and forwards only logs containing the keyword "TRAFFIC" to the SIEM over TCP.

siem_listener.py acts as the SIEM, listening for and displaying only the forwarded "TRAFFIC" logs.

This shows log ingestion, storage, filtering, and forwarding in a minimal (macOS-friendly) setup.
