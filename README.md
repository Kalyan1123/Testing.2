if(empty(triggerOutputs()?['body/_psquad_relatedlcm2_value']), outputs('Get_Host_email')?['body/psquad_email'], concat(outputs('Get_Host_email')?['body/psquad_email'], ';', outputs('GetCoHostEmailRow')?['body/psquad_email']))

formatDateTime(triggerOutputs()?['body/psquad_startdatetime'], 'yyyy-MM-ddTHH:mm:ss')

formatDateTime(triggerOutputs()?['body/psquad_enddatetime'], 'yyyy-MM-ddTHH:mm:ss')

Session created. Join here:


Left = empty(triggerOutputs()?['body/_psquad_relatedlcm2_value']), operator = is equal to, right = false.

outputs('Get_Host_email')?['body/psquad_email']

/*"
<div style="font-family:Segoe UI,Arial,sans-serif;color:#201f1e;">
<h2 style="color:#0f6cbd;">Session Created Successfully</h2>
<p>The following session has been scheduled. Details below.</p>
<table style="border-collapse:collapse;width:100%;max-width:600px;">
<tr style="background:#0f6cbd;color:#ffffff;">
<th style="border:1px solid #ccc;padding:10px;text-align:left;">Field</th>
<th style="border:1px solid #ccc;padding:10px;text-align:left;">Details</th>
</tr>
<tr>
<td style="border:1px solid #ccc;padding:10px;font-weight:bold;">Session Name</td>
<td style="border:1px solid #ccc;padding:10px;">[EVENT_TITLE]</td>
</tr>
<tr style="background:#f3f2f1;">
<td style="border:1px solid #ccc;padding:10px;font-weight:bold;">Technology</td>
<td style="border:1px solid #ccc;padding:10px;">[TECHNOLOGY]</td>
</tr>
<tr>
<td style="border:1px solid #ccc;padding:10px;font-weight:bold;">Description</td>
<td style="border:1px solid #ccc;padding:10px;">[DESCRIPTION]</td>
</tr>
<tr style="background:#f3f2f1;">
<td style="border:1px solid #ccc;padding:10px;font-weight:bold;">Start Date &amp; Time</td>
<td style="border:1px solid #ccc;padding:10px;">[START]</td>
</tr>
<tr>
<td style="border:1px solid #ccc;padding:10px;font-weight:bold;">End Date &amp; Time</td>
<td style="border:1px solid #ccc;padding:10px;">[END]</td>
</tr>
<tr style="background:#f3f2f1;">
<td style="border:1px solid #ccc;padding:10px;font-weight:bold;">Host</td>
<td style="border:1px solid #ccc;padding:10px;">[HOST_EMAIL]</td>
</tr>
<tr>
<td style="border:1px solid #ccc;padding:10px;font-weight:bold;">Co-Host</td>
<td style="border:1px solid #ccc;padding:10px;">[COHOST_EMAIL]</td>
</tr>
<tr style="background:#f3f2f1;">
<td style="border:1px solid #ccc;padding:10px;font-weight:bold;">Optional</td>
<td style="border:1px solid #ccc;padding:10px;">[OPTIONAL_EMAIL]</td>
</tr>
</table>
<p style="margin-top:20px;">
<a href="[JOIN_URL]" style="background:#0f6cbd;color:#ffffff;padding:12px 24px;text-decoration:none;border-radius:4px;display:inline-block;">Join Teams Meeting</a>
</p>
</div>
"
*/

<div style="font-family:Segoe UI,Arial,sans-serif;color:#201f1e;">
<h2 style="color:#0f6cbd;">Session Created Successfully</h2>
<p>The following session has been scheduled. Details below.</p>
<table style="border-collapse:collapse;width:100%;">
<tr style="background:#0f6cbd;color:#ffffff;">
<th style="border:1px solid #ccc;padding:10px;text-align:left;">Session Name</th>
<th style="border:1px solid #ccc;padding:10px;text-align:left;">Technology</th>
<th style="border:1px solid #ccc;padding:10px;text-align:left;">Description</th>
<th style="border:1px solid #ccc;padding:10px;text-align:left;">Start Date &amp; Time</th>
<th style="border:1px solid #ccc;padding:10px;text-align:left;">End Date &amp; Time</th>
</tr>
<tr>
<td style="border:1px solid #ccc;padding:10px;">[EVENT_TITLE]</td>
<td style="border:1px solid #ccc;padding:10px;">[TECHNOLOGY]</td>
<td style="border:1px solid #ccc;padding:10px;">[DESCRIPTION]</td>
<td style="border:1px solid #ccc;padding:10px;">[START]</td>
<td style="border:1px solid #ccc;padding:10px;">[END]</td>
</tr>
</table>
<p style="margin-top:20px;">
<a href="[JOIN_URL]" style="background:#0f6cbd;color:#ffffff;padding:12px 24px;text-decoration:none;border-radius:4px;display:inline-block;">Join Teams Meeting</a>
</p>
</div>



outputs('Create_a_Teams_meeting')?['body/onlineMeeting/joinUrl']
