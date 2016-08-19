# Open Event
[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/fossasia/open-event?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Mailing List](https://img.shields.io/badge/Mailing%20List-FOSSASIA-blue.svg)](https://groups.google.com/forum/#!forum/open-event)

The Open Event Project offers event managers a platform to organize all kinds of events including concerts, conferences, summits and regular meetups. The components support organizers in all stages from event planning to publishing, marketing and ticket sales. Automated web and mobile apps help attendees to get information easily. There are four components of the project:

1. The Open Event Format Definition [[JSON Schema Sample](/sample/)]

2. The Open Event Orga Server [[Repository](https://github.com/fossasia/open-event-orga-server)]

3. The Open Event Android App Generator [[Repository](https://github.com/fossasia/open-event-android)]

4. The Open Event Web App Generator [[Repository](https://github.com/fossasia/open-event-webapp)]

The source code of each component has its own repository and technology stack. The software applications can be hosted as stand alone solutions or they can be integrated as microservices into the Open Event Orga Server through APIs. 

The Open Event project was originally started to support the organization of the [FOSSASIA OpenTechSummit](http://fossasia.org) and is maintainted by the FOSSASIA community.

## Open Event Repository

This repository holds the **JSON Schema** sample implementation in the [/sample](/sample/) folder, that is used across all projects for testing. We keep a) Zip files that include all JSON files with binary media data and b) the uncompressed files that can act as APIs substitutes to test applications.

## Communication

Please join our mailing list to discuss questions regarding the project: https://groups.google.com/forum/#!forum/open-event

Our chat channel is here: https://gitter.im/fossasia/open-event

## Project Components

### Open Event Format Definition

The Open Event project enables the exchange of data between all components as well as with other services through a standardized Format. The Open Event repository provides a sample implementation of the format. It includes JSON files for all relevant event information and binary data for images and audio files.

Repository: https://github.com/fossasia/open-event   

Chat Channel: https://gitter.im/fossasia/open-event

### Open Event Organizer Server

The Open Event Orga Server enables organizers to manage events from concerts to conferences and meetups. It offers features for events with several tracks and venues. Event managers can create invitation forms for speakers and build schedules in a drag and drop interface. The event information is stored in a database, which can be a sqlite db file or saved in json itself. The system provides API endpoints to fetch the data, and to modify and update it. Organizers can import and export event data in a standard compressed file format that includes the event data in JSON and binary media files like images and audio

Repository: https://github.com/fossasia/open-event-orga-server   

Chat Channel: https://gitter.im/fossasia/open-event-orga-server

### Open Event Android App
 
The Open Event Android project consists of two components. The **App Generator** is hosted web application, that is hosted on a server and generates an event Android app from a zip with JSON and binary files ([examples here](http://github.com/fossasia/open-event)) or through an API. The second component we are developing in the project is generic **Android app** - the output of the app generator. The mobile app can be installed on any Android device for browsing information about the event. Updates can be made automatically through API endpoint connections from an online source (e.g. server), which needs to defined in the provided event zip with the JSON files. The Android app has a standard configuration file, that sets the details of the app (e.g. color scheme, logo of event, link to JSON app data).   

Repository: https://github.com/fossasia/open-event-android

Chat Channel: https://gitter.im/fossasia/open-event-android

### Open Event WebApp

The Open Event Web App project has two components a) a event website generator and b) the actual generated website output. The web generator application can generate event websites by getting data from event JSON files and binary media files, that are stored in a compressed zip file. You can also access the application through a Rest API. Websites that are generated by the "web app generator" can be uploaded to any web location, e.g. on Github pages or any server (e.g. via ftp).  

Repository: https://github.com/fossasia/open-event-webapp

Chat Channel: https://gitter.im/fossasia/open-event-webapp

## License

This repository is licensed under the GNU General Public License v3. A copy of LICENSE.md should be present along with the source code. To obtain the
software under a different license, please contact FOSSASIA.
