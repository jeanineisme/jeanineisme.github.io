# Cybersecurity Projects 

Showcasing hands-on projects in cybersecurity, demonstrating expertise in network security, threat analysis, and system optimization. Each project reflects my commitment to safeguarding digital environments through innovative solutions.

## Creating a SOC

> Created a security operations center (SOC) by deploying a security and event manager (SIEM) the monitors and generates alerts for all the devices in my personal home lab. Set up an intelligence feed that sends the SIEM commonly seen and newly found indicators of compromise.

##### Technology
- Microsoft Azure
  - Virtual Machine (VM): Windows 10 Pro
  - Microsoft Sentinel resource group to create log log analytics workspace

##### Process
1.  Set up the Windows 10 Pro VM in Azure. Left RDP open on port 3389 on purpose.
2.  Created and added log analytics workspace in Sentinel, adding it to the resource group that houses all of my resources (VMs, SIEM tools, etc.).
3.  Added VM event logs to the log analytics workspace.This will send it to the Sentinel instance.
    *  Set up Data connector with Windows Security Event via AMA in the Content Hub.
    *  Set up data collection rule.
4.   Created a Sentinel rule that checks for sign-ins via RDP (successful brute force attempts) and generate an alert.
    ![SecurityEventRule](securityeventrule.png)

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
