# AI-SOC-Analyst

AI-Automated SOC Analyst: Threat Detection & LLM Investigation

This project demonstrates a functional AI-driven Security Operations Center (SOC) pipeline that automates the detection and analysis of network threats. Using a Python-based automation script on a Kali Linux internal server, the system captures live network traffic via tshark and monitors for suspicious volume thresholds, such as ICMP floods from an attacking CSI Linux machine. Once a threshold—configured at 40 packets—is exceeded, the script automatically parses the traffic, identifies the offending source IP, and generates a structured JSON alert.  


The core innovation lies in the integration with the Airia.ai platform, where a "Junior SOC Analyst" AI agent is trained with a specific SOC playbook to investigate these alerts. Upon receiving the JSON telemetry, the agent performs a high-speed risk assessment, calculates a severity score based on packet volume, and maps the activity to potential threat levels. The final output provides the human analyst with a comprehensive executive summary, a critical risk rating (reaching 90/100 in testing), and actionable mitigation steps like IP blocking and tier-2 escalation.  
