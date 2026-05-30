# Test Cases

## Test 1 - Probe Attack
Input: Protocol: TCP, Service: http, Duration: 0,
Source bytes: 491, Destination bytes: 0, Flag: S0

Output:
- CLASSIFICATION: Probe
- CONFIDENCE: 85%
- ATTACK TYPE: Port Scanning
- REASON: TCP SYN packet with no response...

## Test 2 - Normal Traffic
Input: Protocol: TCP, Service: http, Duration: 181,
Source bytes: 5450, Destination bytes: 5450, Flag: SF

Output:
CLASSIFICATION: Normal 
CONFIDENCE: 95% 
ATTACK TYPE: None 
REASON: The traffic shows a typical HTTP session with a balanced exchange of data between the source and destination.


## Test 3 - DoS Attack
Input: Protocol: TCP, Service: http, Duration: 0,
Source bytes: 491, Destination bytes: 0, Flag: S0,
High frequency requests

Output: 
CLASSIFICATION: DoS 
CONFIDENCE: 90% 
ATTACK TYPE: Denial of Service (SYN Flood) 
REASON: The repeated TCP SYN packets (Flag: S0) from the same source IP address with no corresponding responses and a very short duration suggest a SYN flood attack, which is a common form of Denial of Service (DoS) attack.
