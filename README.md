# Network Intrusion Detection Agent
## AICTE IBM SkillsBuild Project 2026

### Problem Statement
PS 40 - Network Intrusion Detection using AI

### Objective
Build an AI agent that analyzes network traffic 
and classifies it as Normal, DoS, Probe, R2L, or U2R attack.

### Technology Used
- IBM Watsonx.ai (Dallas region)
- IBM Granite 4.0 H Small model
- IBM Cloud Lite services

### How it works
1. User inputs network traffic details
2. IBM Granite LLM analyzes the pattern
3. Agent returns: Classification, Confidence %, Attack Type, Reason

### Sample Output
Input: TCP traffic with S0 flag, 0 destination bytes
Output:
- CLASSIFICATION: Probe
- CONFIDENCE: 85%
- ATTACK TYPE: Port Scanning
- REASON: TCP SYN packet with no response indicates port scanning

### Demo Screenshots

sample 1
<img width="820" height="315" alt="image" src="https://github.com/user-attachments/assets/29b99046-5a8f-4d38-af5d-7646d34f6d4e" />

sample 2
<img width="854" height="232" alt="image" src="https://github.com/user-attachments/assets/0e4b8ec4-674a-49f6-a489-ee29ca920200" />

sample 3
<img width="829" height="246" alt="image" src="https://github.com/user-attachments/assets/415e8afe-419f-44dc-b3b3-4755f1e3555f" />


### Project by
Name: Mohamed Zubeir
Program: AICTE IBM SkillsBuild Internship 2026
