if(empty(triggerOutputs()?['body/_psquad_relatedlcm2_value']), outputs('Get_Host_email')?['body/psquad_email'], concat(outputs('Get_Host_email')?['body/psquad_email'], ';', outputs('GetCoHostEmailRow')?['body/psquad_email']))

formatDateTime(triggerOutputs()?['body/psquad_startdatetime'], 'yyyy-MM-ddTHH:mm:ss')

formatDateTime(triggerOutputs()?['body/psquad_enddatetime'], 'yyyy-MM-ddTHH:mm:ss')

Session created. Join here:
