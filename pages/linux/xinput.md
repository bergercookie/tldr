# xinput

> List available input devices, query information about a device and change input device settings.

- List all input devices:

`xinput list`

- Set the acceleration speed for a mouse:

`xinput --set-prop {{id}} 'libinput Accel Speed' {{vall-between-0-1}}

- Disable an input:

`xinput disable {{id}}`

- Enable an input:

`xinput enable {{id}}`

- Disconnect an input from its master:

`xinput float {{id}}`

- Reattach an input as slave to a master:

`xinput reattach {{id}} {{master_id}}`
