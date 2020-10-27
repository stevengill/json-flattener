# json-flattener

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/stevengill/json-flattener/tree/main)

A server that receives json payloads, flattens the keys and sends this new payload to a slack webhook

## Learnings

- Michael and Steve learned about Workflow Builder Webhooks
- Michael learned about LiveShare in Visual Code
- Workflow Builder returns HTTP 400 and `Received a webhook request that was missing a required field` error when a configured variable is missing from the incoming payload. 
- Workflow Builder returns HTTP 400 and `invalid_field` error if incoming value is not a string.
- Workflow Builder / Slackbot only unfurls a URL once, but simple workflows may want to leverage unfurls to create beautiful messages with ease.
- Workflow Builder does not support the use of variables in hyperlinks
- Workflow Builder does not support the use of block kit elements

## Roadmap

- Help user preview flattened keys and copy them to their clipboard for use in Workflow Builder. Build UI to paste source JSON payload and preview it from the landing page.