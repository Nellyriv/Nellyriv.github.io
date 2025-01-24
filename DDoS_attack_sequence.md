'''mermaid
sequenceDiagram
participant Attacker
participant BotNet
participant WebServer
participant Firewall
Attacker ->> BotNet: Rents/Builds infected machines 
Attacker ->> WebServer: Launches attack
BotNet ->> WebServer: Overwhelm with traffic and requests
WebServer->> Firewall: Server slows down or crashes
Firewall->> WebServer: inspects traffic and protects from malicious requests by blocking IP

#DDoS 
in a DDoS attack the attacker has to plan and buy/build a network of bots and find a server they want to target.
The attacker will then launch the attack from their own server. The BotNet will be sent to the targeted WebServer
and will overwhelm it with requests so real users can't access it. This affects usability and server speed which triggers
the firewall to look for malicious activity from suspicious users using rate limiting and load balancing.
'''
