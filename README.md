# Network-Automation-With-My-Home-Network-
automating my home network using Ansible, Playbooks, and YAML
<h1>Network Automation Lab</h1>

<h2>Description</h2>
In this lab, I am using Network Automation via Cisco Meraki, Ansible, Playbooks, and Yaml to automate my Home Lab.
<br />


<h2>Languages and Utilities Used</h2>

- Bash and linux terminal</b> 

<h2>Environments Used </h2>

- <b>Linux/b> 

<h2>Program walk-through:</h2>

<p align="center">
Generate an API Key to connect to Cisco Meraki's Dashboard. : <br/>
<img src="https://i.imgur.com/TvBBX08.png"/>
<br />
<br />
Created an ansible playbook:  <br/>
<img src="https://i.imgur.com/eMdUw91.png"/>
<br />
<br />
executed the playbook in terminal to verify it works: <br/>
<img src="https://i.imgur.com/DlEGMJ7.png"/>
<br />
<br />
Created a playbook that is going to automate my home lab (just need to finish by inoutting correct date) (in progress...):  <br/>
<img src="https://i.imgur.com/nQtTxIZ.png"/>
<br />
Brief explanation of whats going on in the playbook: 
    The first task Get Organization Networks, returns a list of networks in the organization.
    The second task Filter networks with "wireless" productTypes returns a filtered list of networks that have "wireless" in their product types list.
    The third task creates the SSID for each network. Notice the loop and loop_control parameters. The task will be repeated with a different network ID (item.id).
  <br/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
