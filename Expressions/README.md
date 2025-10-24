Expression for the Compose step to extract the recipient email address:
trim(substring(triggerOutputs()?['body/body'], add(indexOf(triggerOutputs()?['body/body'], 'Email: '), 7), sub(indexOf(triggerOutputs()?['body/body'], 'Phone Number:'), add(indexOf(triggerOutputs()?['body/body'], 'Email: '), 7))))
