<h1>Work Order notification and Documentation automation</h1>

<h2>Challanges in workplace</h2>
<p>Conservatively, paperwork involving tools repairs and techfaxes was recorded/printed in a paper and stored in a cabinet. This was the way for Sperry R&M since 80's</p>
<p><em>If it's working, don't change it</em></p>
<p>Traditional documentation require hardcopy proved to be unsustainable and leads to tons of paper to work with, this leads to the needs for storage to store such document and compliance towards company data retention.</p><p>For Kuwait RNM RSS team, we have shifted all the documentation from being paper dependent to paper free since 2018.</p><p> Paperwork that was uploaded into SAP is also stored in Local Network Folder. This subsequently allow faster data retrieval in the event of an incident involving failure investigation or simply updating the tool information. By migrating from hardcopy to softcopy, the process has saved tons of hours and space. This also increase the team productivity and efficiency in folds.</p> 
<p>Using the Local Network Folder as a server for storage purposes also increase efficiency of the documentation control and mitigate the rate of missing infromation while recording the repair process of tools.</p>
<p>This however can be improved further.</p>
<h2>Addressing the oppurtunity for change</h2>
<p>The Local Network Folder utilisation proved to have it's pros and cons.</p>
<h3>Advantages</h3>
<ul>
    <li>Faster data transfer.</li>
    <li>Large size of file can be stored.</li>
    <li>Easily accessible using Windows environment.</li>
    <li>Maintained by Hal IT Pros.</li>
</ul>
<h3>Disadvantages</h3>
<ul>
    <li>Require special access for full read and write and often, request for such access take forever.</li>
    <li>Server down during update.</li>
    <li>Require workstation to access the Local Network.</li>
    <li>File sharing limited to domestic users.</li>
</ul>
<p>To counter these challange, I purpose an alternative solution which is Cloud base server that are readily available for Hal employee such as Microsoft SharePoint and OneDrive complemented with Kuwait RSS RNM PowerApps.</p>


<h1>Objective</h1>
<h2>To create working system of documentation Automation</h2>
<p>By having an automated documentation control, the process of data capture can be delegated to the right person and proper identifiable folder structure.</p> <p>For example, in SharePoint, the document that were dropped from particular person will be displayed as<tt style="font-size:1.2em"> modified by</tt>.</p>
<img src="/Images/Screenshot 2022-02-04 at 9.06.52 PM.png">
<p>Having the document ownership is very important features nowadays and SharePoint product enable the posibility of greater control of documentation.</p>
<p>On top of that, a document version control called as <tt style="font-size:1.2em"> Version history</tt> will provide greater transparency and better backup for document when things goes awry.</p>
<img src="/Images/Screenshot 2022-02-04 at 9.12.14 PM.png">
  
<h3>Benefit of utilising SharePoint as document server</h3>
<ul>
    <li>Power Automate and PowerApps readily avaiable for automation experience.</li>
    <li>Large size of file can be stored.</li>
    <li>File can be accessed anytime and anywhere globally.</li>
    <li>Maintained by Microsoft IT Pros.</li>
    <li>Require minimal setup for working environment ie: desktop are not needed to access and share document.</li>
</ul>
 <h1>Implementation</h1>
 <h2>PowerApps</h2>
 <h3>Kuwait RSS RNM Apps</h3>
<img src="/Images/Screenshot 2022-02-04 at 9.45.23 PM.png" height="500px" width="auto">


<p>This application was design and built for iPad usage. By utilising the PowerApps modern features, creating and retrieving paperwork through dozuki is simplified and made easy.</p>
<h3>Pseudo</h3>
<p> 
    <p><tt>Start</tt></p>
    <p><tt>Work Order created inside PowerApps</tt></p>
    <p><tt>&emsp;&emsp;PowerApps will update excel in SharePoint and create SharePoint List</tt></p>
    <p><tt>&emsp;&emsp;Main and sub Tech notified that the new work order created through Power Automate</tt></p>
    <p><tt>&emsp;&emsp;&emsp;&emsp;Tech work on that work order and drop through link generated from PowerApps</tt></p> 
    <p><tt>&emsp;&emsp;&emsp;&emsp;Automatically trigger notification from Outlook/Teams indicating work has done</tt></p>
    <p><tt>&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;SharePoint List updated with new value indicating the work has done</tt></p>
    <p><tt>&emsp;&emsp;Main tech provide sub number and automate will extract document in PowerApps</tt></p>
    <p><tt>&emsp;&emsp;&emsp;&emsp;File name will be appended with folder string for uniformity through automate</tt></p>
    <p><tt>&emsp;&emsp;&emsp;&emsp;Automatically trigger notification from Outlook/Teams indicating work has done</tt></p>
    <p><tt>&emsp;&emsp;Compile in ZIP and copy into SAP</tt></p>
    <p><tt>End</tt></p>
</p>
  

<img src="/Images/Screenshot 2022-02-04 at 10.27.35 PM.png" height="500px" width="auto">

<p>For more information, contact <a mailto="erwan.fadlys@gmail.com">erwan.fadlys@gmail.com.</a>
 
 
