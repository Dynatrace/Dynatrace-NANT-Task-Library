<html xmlns="http://www.w3.org/1999/xhtml">
<head>
    <title>NANT Task Library</title>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8"/>
    <meta http-equiv="X-UA-Compatible" content="IE=EmulateIE8" />
    <meta content="Scroll Wiki Publisher" name="generator"/>
    <link type="text/css" rel="stylesheet" href="css/blueprint/liquid.css" media="screen, projection"/>
    <link type="text/css" rel="stylesheet" href="css/blueprint/print.css" media="print"/>
    <link type="text/css" rel="stylesheet" href="css/content-style.css" media="screen, projection, print"/>
    <link type="text/css" rel="stylesheet" href="css/screen.css" media="screen, projection"/>
    <link type="text/css" rel="stylesheet" href="css/print.css" media="print"/>
</head>
<body>
                <h1>NANT Task Library</h1>
    <div class="section-2"  id="8651512_NANTTaskLibrary-Overview"  >
        <h2>Overview</h2>
    <p>
            <img src="images_community/download/attachments/8651512/icon.png" alt="images_community/download/attachments/8651512/icon.png" class="confluence-embedded-image" />
        The Download Package includes a .NET Library that implements several tasks to be used by NAnt scripts.    </p>
    <div class="tablewrap">
        <table>
<thead class=" "></thead><tfoot class=" "></tfoot><tbody class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
Name    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<strong class=" ">NAnt Task Library</strong>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
dynaTrace Version    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
3.x, 4.x, 5.x, 6.0    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Author    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
dynaTrace software    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
License    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="attachments_5275722_2_dynaTraceBSD.txt">dynaTrace BSD</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Support    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="https://community/display/DL/Support+Levels#SupportLevels-Supported">Supported</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Download    </p>
            </td>
                <td rowspan="1" colspan="1">
    <ul class=" "><li class=" ">    <p>
<a href="attachments_174751927_1_dynatrace-nant.plugin-6.0.0.6733.zip">NANT Plugin for dynaTrace 6.0</a>    </p>
</li><li class=" ">    <p>
<a href="attachments_150700314_1_dynatrace-nant.plugin-5.6.0.5713.zip">NANT Plugin for dynaTrace 5.6</a>    </p>
</li><li class=" ">    <p>
<a href="attachments_121569600_1_dynatrace-nant.plugin-5.5.0.5226.zip">NANT Plugin for dynaTrace 5.5</a>    </p>
</li><li class=" ">    <p>
<a href="attachments_100925540_1_dynaTrace_NANT_Task_v5.zip">NANT Tasks for dynaTrace 5</a>  (includes a sample build file)    </p>
</li><li class=" ">    <p>
<a href="attachments_89718913_1_dynaTrace_NANT_Task_v4.2.zip">NANT Tasks for dynaTrace 4.2</a>  (includes a sample build file)    </p>
</li><li class=" ">    <p>
<a href="attachments_67829826_1_dynaTrace_NANT_Task_v41.zip">NANT Tasks for dynaTrace 4.1</a>  (includes a sample build file)    </p>
</li></ul>            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Older Versions    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="https://community/display/DL/NAnt+Task+Library+for+2.6">NAnt Task Library for 2.6</a>    </p>
            </td>
        </tr>
</tbody>        </table>
            </div>
    </div>
    <div class="section-2"  id="8651512_NANTTaskLibrary-Description"  >
        <h2>Description</h2>
    <p>
The Download Package includes a .NET Library that implements several tasks to be used by NAnt scripts.    </p>
    <p>
Following tasks can be executed:    </p>
<ul class=" "><li class=" ">    <p>
Start, Stop or Restart the dynaTrace Server    </p>
</li><li class=" ">    <p>
Start and Stop Session Recording    </p>
</li><li class=" ">    <p>
Change Active Configuration    </p>
</li><li class=" ">    <p>
Set Test Information (new in dT 3.5)    </p>
</li></ul>    <p>
This library makes use of the <a href="https://community/display/DL/.NET+Command+Library">.NET Command Library</a>.    </p>
    </div>
    <div class="section-2"  id="8651512_NANTTaskLibrary-Installation"  >
        <h2>Installation</h2>
    <div class="confbox panel">
    <ol class=" "><li class=" ">    <p>
Save the attached file locally to the computer where the dynaTrace Client is installed.    </p>
</li><li class=" ">    <p>
Unzip the file.    </p>
</li><li class=" ">    <p>
Copy the extracted dlls to a directory where it can be picked up by NAnt when executing your build scripts    </p>
</li><li class=" ">    <p>
View the extracted sample_nant.xml file. It shows how you can load the new build tasks in your NAnt scripts    </p>
</li></ol>    </div>
    </div>
    <div class="section-2"  id="8651512_NANTTaskLibrary-Usage"  >
        <h2>Usage</h2>
    <p>
You have to register the new Build Tasks with the UseTask configuration entry in your build scripts like this:    </p>
    <div class="confbox programlisting">
                <div class="content">
        <pre><code>&lt;loadtasks assembly=&quot;dynaTrace.NANT.Task.dll&quot; /&gt;</code></pre>
        </div>
    </div>
    <p>
The following tasks with the listed properties can now be used in your NAnt scripts:    </p>
    <p>
<strong class=" "> <i class=" ">StartSessionRecordingTask</i> </strong>    </p>
<ul class=" "><li class=" ">    <p>
ProfileName: (mandatoy) - specifies the System Profile you want to start recording on    </p>
</li><li class=" ">    <p>
RecordSessionName: (optional) - allows you to define the name of the recorded session    </p>
</li><li class=" ">    <p>
dtVersion: (optional) - this is the dynaTrace Client Version that you want to use. In case multiple versions of dynaTrace are installed you use this to connect to the correct version    </p>
</li><li class=" ">    <p>
dtInstallDir: (optional) - this is the dynaTrace Client Installation directory. If not specified the value is read from the registry    </p>
</li><li class=" ">    <p>
ServerName: (optional) - the dynaTrace Server Hostname to connect to. Default: localhost    </p>
</li><li class=" ">    <p>
Username: (optional) - the username to connect to the dynaTrace Server. Default: admin    </p>
</li><li class=" ">    <p>
Password (optional) - the password to connect to the dynaTrace Server. Default: admin    </p>
</li></ul>    <p>
<strong class=" "> <i class=" ">StopSessionRecordingTask</i> </strong>    </p>
<ul class=" "><li class=" ">    <p>
ProfileName: (mandatory)    </p>
</li><li class=" ">    <p>
dtVersion, dtInstallDir, ServerName, Username, Password: see description of StartSessionRecording    </p>
</li></ul>    <p>
<strong class=" "> <i class=" ">SetActiveConfigurationTask</i> </strong>    </p>
<ul class=" "><li class=" ">    <p>
ConfigurationName: (mandatory) - configuration name to switch to    </p>
</li><li class=" ">    <p>
ProfileName: (mandatory) - System Profile where you want to switch the active configuration    </p>
</li><li class=" ">    <p>
dtVersion, dtInstallDir, ServerName, Username, Password: see description of StartSessionRecording    </p>
</li></ul>    <p>
<strong class=" "> <i class=" ">ServerServiceTask</i> </strong>    </p>
<ul class=" "><li class=" ">    <p>
ServiceCommand: (mandatory). Allows one of the following values: startup, restart, shutdown    </p>
</li><li class=" ">    <p>
dtVersion, dtInstallDir, ServerName, Username, Password: see description of StartSessionRecording    </p>
</li></ul>    <p>
<strong class=" "> <i class=" ">ConfigureApplicationTask</i> </strong>    </p>
<ul class=" "><li class=" ">    <p>
Executable: (mandatory). Defines the full path to the executable you want to configure, e.g.: C:\MySample\MyApp.exe    </p>
</li><li class=" ">    <p>
Active: (mandatory). True or False. Allows to switch a configuration active or inactive    </p>
</li><li class=" ">    <p>
AgentName: (optional). Name of the Agent. Default: name of the executable file, e.g.: MyApp.exe    </p>
</li><li class=" ">    <p>
CommandLine: (optional). Command Line that must match the process. Default: empty==any command line value    </p>
</li><li class=" ">    <p>
ServerName: (optional). dynaTrace Servername to let the Agent connect to. Default: localhost    </p>
</li><li class=" ">    <p>
ServerPort: (optional). dynaTrace server port to let the Agent connect to. Default: 9998    </p>
</li><li class=" ">    <p>
LogFile: (optional). location where to store Agent logfile    </p>
</li><li class=" ">    <p>
LogLevelLife: (optional). LogLevel for the Log File. Possible Values: LOG_NONE, LOG_SEVERE, LOG_WARNING, LOG_INFO, LOG_FINE, LOG_FINER, LOG_FINEST. Default: LOG_NONE    </p>
</li><li class=" ">    <p>
LogLevelConsole: (optional). LogLevel for Console Loggin. Default: LOG_INFO    </p>
</li></ul>    <p>
<strong class=" "> <i class=" ">SetTestInformation</i> </strong> (new in dynaTrace 3.5)    </p>
<ul class=" "><li class=" ">    <p>
VersionMajor: Major Version of your Software    </p>
</li><li class=" ">    <p>
VersionMinor: Minor Version of your Software    </p>
</li><li class=" ">    <p>
VersionRevision: Revision of your Software    </p>
</li><li class=" ">    <p>
VersionBuild: Build Number of your Software    </p>
</li><li class=" ">    <p>
VersionMilestone: Milestone of your Software    </p>
</li><li class=" ">    <p>
Marker: Marker Name that should be shown in the chart for this test execution    </p>
</li><li class=" ">    <p>
Agent Group: The name of the agent group that this test information should be set for. Applied to all agent groups if not set.    </p>
</li><li class=" ">    <p>
SystemProfile: The name of the system profile that this test information should be set for.    </p>
</li><li class=" ">    <p>
CustomProperty: A custom property that should be set for this test information    </p>
</li></ul>    </div>
    <div class="section-2"  id="8651512_NANTTaskLibrary-Internals"  >
        <h2>Internals</h2>
    <p>
The Library uses the dynaTrace.Command.dll which is installed with the dynaTrace Server. dynaTrace.Command.dll uses the dynaTrace Web Service interfaces. For every dynaTrace.Command.dll call the library creates an EventLog Entry with detailed information about the command line arguments that were passed. This should help with troubleshooting.    </p>
    <p>
The task ConfigureApplicationTask needs write access to the HKLM Registry on your local machine. In case your user does not have the appropriate access rights you will run into errors.    </p>
    </div>
    <div class="section-2"  id="8651512_NANTTaskLibrary-SampleNAntScript"  >
        <h2>Sample NAnt Script</h2>
    <p>
The download package includes a sample NAnt file. Check it out for a reference    </p>
    </div>
    <div class="section-2"  id="8651512_NANTTaskLibrary-Attachments"  >
        <h2>Attachments</h2>
    <p>
    </p>
    <div class="tablewrap">
        <table>
<thead class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
&nbsp;    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="NANT_Task_Library.html">File</a>    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="NANT_Task_Library.html">Modified</a>    </p>
            </td>
        </tr>
</thead><tfoot class=" "></tfoot><tbody class=" ">    <tr>
            <td rowspan="1" colspan="1">
                </td>
                <td rowspan="1" colspan="1">
        <p>
File                    <a href="https://community/download/attachments/8651512/dynatrace-nant.plugin-6.0.0.6733.zip?api=v2">dynatrace-nant.plugin-6.0.0.6733.zi&hellip;</a>    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Jul 17, 2014by<a href="    /community/display/~stefan.frandl@compuware.com ">Stefan Frandl</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
                </td>
                <td rowspan="1" colspan="2">
        <p>
    </p>
    <p>
Labels    </p>
<ul class="label-list has-pen "><li class="no-labels-message ">    <p>
No labels    </p>
</li><li class="labels-edit-container ">    <p>
<a href="NANT_Task_Library.html">Edit Labels</a>    </p>
</li></ul>    <p>
    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
                </td>
                <td rowspan="1" colspan="1">
        <p>
ZIP Archive                    <a href="https://community/download/attachments/8651512/dynatrace-nant.plugin-5.6.0.5713.zip?api=v2">dynatrace-nant.plugin-5.6.0.5713.zi&hellip;</a>    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Jan 14, 2014by<a href="    /community/display/~stefan.frandl@compuware.com ">Stefan Frandl</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
                </td>
                <td rowspan="1" colspan="2">
        <p>
    </p>
    <p>
Labels    </p>
<ul class="label-list has-pen "><li class="no-labels-message ">    <p>
No labels    </p>
</li><li class="labels-edit-container ">    <p>
<a href="NANT_Task_Library.html">Edit Labels</a>    </p>
</li></ul>    <p>
    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
                </td>
                <td rowspan="1" colspan="1">
        <p>
ZIP Archive                    <a href="https://community/download/attachments/8651512/dynatrace-nant.plugin-5.5.0.5226.zip?api=v2">dynatrace-nant.plugin-5.5.0.5226.zi&hellip;</a>    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
May 23, 2013by<a href="    /community/display/~stefan.frandl@compuware.com ">Stefan Frandl</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
                </td>
                <td rowspan="1" colspan="2">
        <p>
    </p>
    <p>
Labels    </p>
<ul class="label-list has-pen "><li class="no-labels-message ">    <p>
No labels    </p>
</li><li class="labels-edit-container ">    <p>
<a href="NANT_Task_Library.html">Edit Labels</a>    </p>
</li></ul>    <p>
    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
                </td>
                <td rowspan="1" colspan="1">
        <p>
ZIP Archive                    <a href="https://community/download/attachments/8651512/dynaTrace_NANT_Task_v5.zip?api=v2">dynaTrace_NANT_Task_v5.zip</a>    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Nov 30, 2012by<a href="    /community/display/~wolfgang.gottesheim@compuware.com ">Wolfgang Gottesheim</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
                </td>
                <td rowspan="1" colspan="2">
        <p>
    </p>
    <p>
Labels    </p>
<ul class="label-list has-pen "><li class="no-labels-message ">    <p>
No labels    </p>
</li><li class="labels-edit-container ">    <p>
<a href="NANT_Task_Library.html">Edit Labels</a>    </p>
</li></ul>    <p>
    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
                </td>
                <td rowspan="1" colspan="1">
        <p>
ZIP Archive                    <a href="https://community/download/attachments/8651512/dynaTrace_NANT_Task_v4.2.zip?api=v2">dynaTrace_NANT_Task_v4.2.zip</a>    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Jul 30, 2012by<a href="    /community/display/~stefan.frandl@compuware.com ">Stefan Frandl</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
                </td>
                <td rowspan="1" colspan="2">
        <p>
    </p>
    <p>
Labels    </p>
<ul class="label-list has-pen "><li class="no-labels-message ">    <p>
No labels    </p>
</li><li class="labels-edit-container ">    <p>
<a href="NANT_Task_Library.html">Edit Labels</a>    </p>
</li></ul>    <p>
    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
                </td>
                <td rowspan="1" colspan="1">
        <p>
ZIP Archive                    <a href="https://community/download/attachments/8651512/dynaTrace_NANT_Task_v41.zip?api=v2">dynaTrace_NANT_Task_v41.zip</a>    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Dec 23, 2011by<a href="    /community/display/~wolfgang.gottesheim@compuware.com ">Wolfgang Gottesheim</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
                </td>
                <td rowspan="1" colspan="2">
        <p>
    </p>
    <p>
Labels    </p>
<ul class="label-list has-pen "><li class="no-labels-message ">    <p>
No labels    </p>
</li><li class="labels-edit-container ">    <p>
<a href="NANT_Task_Library.html">Edit Labels</a>    </p>
</li></ul>    <p>
    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
                </td>
                <td rowspan="1" colspan="1">
        <p>
ZIP Archive                    <a href="https://community/download/attachments/8651512/dynaTrace_NANT_Task_v4.zip?api=v2">dynaTrace_NANT_Task_v4.zip</a>    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Jul 21, 2011by<a href="    /community/display/~andreas.grabner@compuware.com ">Andreas Grabner</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
                </td>
                <td rowspan="1" colspan="2">
        <p>
    </p>
    <p>
Labels    </p>
<ul class="label-list has-pen "><li class="no-labels-message ">    <p>
No labels    </p>
</li><li class="labels-edit-container ">    <p>
<a href="NANT_Task_Library.html">Edit Labels</a>    </p>
</li></ul>    <p>
    </p>
            </td>
        </tr>
</tbody>        </table>
            </div>
<ul class=" "><li class="drop-zone-text hidden ">    <p>
Drag and drop to upload or browse for files    </p>
            <img src="images_community/images/icons/wait.gif" alt="images_community/images/icons/wait.gif" class="plugin_attachments_dropzone_uploadwaiticon" />
        </li></ul>    <p>
Upload fileFile description<a href="https://community/pages/downloadallattachments.action?pageId=8651512">Download All</a>    </p>
    <p>
    </p>
    </div>
            </div>
        </div>
        <div class="footer">
        </div>
    </div>
</body>
</html>