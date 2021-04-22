> Arduino command line interface 
> More information: <https://github.com/arduino/arduino-cli>

- update index (first thing after install):

`arduino-cli core update-index`

- List all boards:

`arduino-cli board list`

- List all available boards for the given arch:

`arduino-cli board listall`

- Search for a new core to install:

`arduino-cli core search {{arduino nano}}

- Install a core (do this after updating the index):

`arduino-cli core install {{esp8266:esp8266`}}

- Compile current sketch:

`arduino-cli compile --fqbn {{esp8266:esp8266:huzzah}} .`

- Upload current sketch:

`arduino-cli upload -p /dev/ttyUSB0 --fqbn {{esp8266:esp8266:huzzah}} .`

- Search for libraries:

`arduino-cli lib search debouncer`

- Install libary:

`arduino-cli lib install {{FTDebouncer}`}

- Create boilerplate for new sketch:

`arduino-cli sketch new {{my_project`}}

