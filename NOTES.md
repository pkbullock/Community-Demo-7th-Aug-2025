# Call Notes

## PREP Only


```bash
npm install -g @microsoft/m365agentstoolkit-cli
atk -h
```

## FORK

- fork the repo
- in GitHub codespaces, open in repo with the agent
- git clone the new repo
	- git clone https://github.com/pkbullock/copilot-pro-dev-samples

- open the repo with codespaces e.g. code .
- should open in new window
- copy the agent to the new repo

## Sequence

### M365 Agents Extension

| Action | Setting |
|----|----|
| Target Folder | /workspaces/Community-Demo-7th-Aug-2025/Agent |
| App Name | PnP Script Samples Agent |
| App Type | Declarative Agent |

### CLI Method

Use CLI for Microsoft 365 Agents Toolkit, create the agent

```bash
atk new --capability "declarative-agent" --app-name "PnP Script Samples Agent" -folder "Agent" --interactive false --with-plugin no 
atk auth login m365 #(this doesn't work in codespaces due to localhost usage)
atk provision
```

> Note: Auth Token cannot handle the codespaces environment. Sad face!


### Demo in Copilot Pro Dev Samples (No Demo Time)

> Note: Work around - copy the demo time files to the cloned repo


- Find the new Sample
- Create an assets folder
- Copy in sample.json file
- Update sample.json file
	- Replace Placeholders

- Update Readme.md
	- Use Template, rename current to .old
	- Copy template
	- Copy fragments over to the sample