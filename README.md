<!-- ![](https://github.com/<OWNER>/<REPOSITORY>/workflows/<WORKFLOW_NAME>/badge.svg) -->
![GitHub CI workflow status](https://github.com/kaizoku-oh/lota/workflows/Build/badge.svg)
![GitHub Release workflow status](https://github.com/kaizoku-oh/lota/workflows/Build/badge.svg)
![GitHub release](https://img.shields.io/github/v/release/kaizoku-oh/lota)
![GitHub issues](https://img.shields.io/github/issues/kaizoku-oh/lota)
![GitHub top language](https://img.shields.io/github/languages/top/kaizoku-oh/lota)
![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)

![Twitter follow](https://img.shields.io/twitter/follow/kaizoku_ouh?style=social)

# LOTA: Logging Over The Air

LOTA is a remote logging system based on ESP32, making remote logging and debugging in robotics applications easier. It does this by connecting to the serial port of any embedded system and redirects all received logging data to all connected websocket clients.

## Getting Started 🚀

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

* To get started you need to have a local development environment for ESP-IDF including ESP32 toolchain and ESP_IDF, all instructions are found in Espressif Getting started guide.
See [website](https://docs.espressif.com/projects/esp-idf/en/latest/get-started/) for ESP-IDF setup instructions.

* Once your environment is ready you need to add the websocket component to esp-idf, you do this by cloning the component into the esp-idf components path.

```
cd $IDF_PATH/components
git clone https://github.com/Molorius/esp32-websocket
```

Note that $IDF_PATH is your ESP-IDF setup directory.
Usually: /home/username/esp/esp-idf

### Prerequisites 📋

To use this project you just need a couple of things.

#### Hardware:

* An ESP32 board
* USB cable - USB A / micro USB B
* Computer running Windows, Linux, or macOS

#### Software:

* Development environment for ESP-IDF. see Getting Started section.
* Code editor like vscode.

### Installing

Just clone the project repo and plug in your esp32 and flash it.

```
git clone https://github.com/kaizoku-619/lota
cd lota
make flash
```

Once your esp32 is flashed successfully, connect to its AP named ESP32 AP with the password opensesame, open up your browser and navigate to 192.168.4.1 you should see the lota dashboard.

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Bayrem Gharsellaoui** - *Initial work* - [kaizoku-619](https://github.com/kaizoku-619)
* **Ridha Mastouri** - *Initial work* - [MSTR-LNX](https://github.com/MSTR-LNX)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* This project uses the [esp32-websocket](https://github.com/Molorius/esp32-websocket) component developed by [Molorius](https://github.com/Molorius)
* Inspiration
* etc
