# Azure-RBAC-for-Sentinel

What we will do now is how to assign roles in Azure. What we will do is go to <b>Resource groups</b> and select the resource group where our Sentinel workspace resides. In my case I only have one resource group, so we select it.

 <img src="https://i.imgur.com/PAGjaHq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

Then we go to <b>Access Control (IAM)</b> and click on <b>Role assignments</b>.

 <img src="https://i.imgur.com/s87t6tb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

Under Role Assignments, what we can actually see is, first of all, the role assignments that are existing in the subscription. We can also see there is a limit of 4,000 role assignments per subscription. That is something we can actually increase by raising a support request if we run into those limits. I currently have 2 role assignments but because we want to add a new role assignment we will click on <b>Add</b> and 
click on <b>Add role assignment</b>

 <img src="https://i.imgur.com/r36IQ0A.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

What we can then do is search for Sentinel. All the Sentinel roles will show up, so what we will do is click on <b>Sentinel Contributor</b> and click on <b>next</b>.

<img src="https://i.imgur.com/zwsQhHr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

Then under the <b>Members</b> plate, what we can actually do is we can decide whether we want to assign this access to a user, group or service principle that is the first option, or to go with the managed identity.
Manage identity is something that we can and should utilize when we build, for example automation in Sentinel or when we want to assign permissions and especially roles therefore to Azure resources, but in this case we want to assign the Sentinel Contributor role to a person that works in our SOC, and what we will do to do that is we will click on <b>Select Members</b>.

<img src="https://i.imgur.com/eSHFXeo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

In this case I will select my name but you can also select your local user and then click on <b>Select</b>.

<img src="https://i.imgur.com/ed5aFHa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

As you can see, the user is showing up on the members and then all we need to do is click on <b>Review + assign,</b>.

<img src="https://i.imgur.com/rTsnuKI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

Then we get the overview see, which role we are assigning, what is the scope in this case because we did it directly in the resources group. The scope of this role assignment is also tied to the resource group and 
we see which members is actually affected. We click on <b>Review + assign</b>.

<img src="https://i.imgur.com/cyxIfCa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

This is your first role assignment. 

<img src="https://i.imgur.com/fhJPT3b.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
